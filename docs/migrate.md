# Mage Migrate 1.9.4 to 2.x

------------

> vendor/magento/module-store/Model/StoreRepository.php

```
// Around line 74
        if ($store->getId() === null) {

// Add this to see a backtrace
            // debug_print_backtrace();

// Add this to see the store code causing the issue: (code:{$code})
            throw new NoSuchEntityException(
                __("The store (code:{$code}) that was requested wasn't found. Verify the store and try again.")
            );
        }

// .......
// Around line 114, same kind of thing...

        if ($store->getId() === null) {

            // debug_print_backtrace();

            throw new NoSuchEntityException(
                __("The store ID ({$id}) that was requested wasn't found. Verify the store and try again.")
            );
        }
```

Unhide all Product Images on Product Page

    UPDATE `catalog_product_entity_media_gallery_value` SET `disabled` = '0' WHERE `disabled` = '1';

Disable watermarks and old media-gallery

After Set "No" to Enable Old Media Gallery option in Advanced -> System section in system configuration

    php bin/magento media-gallery:sync

    php bin/magento media-content:sync

    php bin/magento catalog:images:resize

#Change Attribute ID for DESC

    DELETE FROM `catalog_category_entity_text` WHERE `attribute_id` = '363';

    UPDATE `catalog_category_entity_text` SET `attribute_id` = '363' WHERE `attribute_id` = '44';

#Delete OLD Crontab Jobs

    delete from core_config_data where path like 'crontab/jobs%';
