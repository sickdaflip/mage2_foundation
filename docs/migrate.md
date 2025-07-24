# Mage Migrate 1.9.4 to 2.x

------------

> vendor/magento/module-store/Model/StoreRepository.php (Optional)

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

Setup Stores via app/etc/config.php as SCOPES

```
'scopes' => [
        'websites' => [
            'admin' => [
                'website_id' => '0',
                'code' => 'admin',
                'name' => 'Admin',
                'sort_order' => '0',
                'default_group_id' => '0',
                'is_default' => '0'
            ],
            'base' => [
                'website_id' => '1',
                'code' => 'base',
                'name' => 'Base',
                'sort_order' => '0',
                'default_group_id' => '1',
                'is_default' => '1'
            ]
        ],
        'groups' => [
            [
                'group_id' => '0',
                'website_id' => '0',
                'name' => 'Default',
                'root_category_id' => '0',
                'default_store_id' => '0',
                'code' => 'default'
            ],
            [
                'group_id' => '1',
                'website_id' => '1',
                'name' => 'Main Website Store',
                'root_category_id' => '2',
                'default_store_id' => '1',
                'code' => 'main_website_store'
            ]
        ],
        'stores' => [
            'admin' => [
                'store_id' => '0',
                'code' => 'admin',
                'website_id' => '0',
                'group_id' => '0',
                'name' => 'Admin',
                'sort_order' => '0',
                'is_active' => '1'
            ],
            'default' => [
                'store_id' => '1',
                'code' => 'default',
                'website_id' => '1',
                'group_id' => '1',
                'name' => 'Default Store View',
                'sort_order' => '0',
                'is_active' => '1'
            ],
            'b2b' => [
                'store_id' => '3',
                'code' => 'b2b',
                'website_id' => '3',
                'group_id' => '3',
                'name' => 'B2B Store View',
                'sort_order' => '10',
                'is_active' => '1'
            ],
            'b2c' => [
                'store_id' => '4',
                'code' => 'b2c',
                'website_id' => '3',
                'group_id' => '3',
                'name' => 'B2C Store View',
                'sort_order' => '20',
                'is_active' => '1'
            ]
        ]
    ]
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
