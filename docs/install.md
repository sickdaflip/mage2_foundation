# Install Mage 2 Dev-Env for this Theme

------------

Installation instructions for the current Magento 2 version.

    composer create-project --repository-url=https://repo.magento.com/ magento/project-community-edition html

add Tools & Elasticsearch 8 (optional)

    composer require magento/data-migration-tool
    composer require magento/module-elasticsearch-8 --update-with-all-dependencies

## install magento

    php bin/magento setup:install \
    --base-url=https://commerce.dev.lan \
    --db-host=localhost \
    --db-name=mariasql1 \
    --db-user=mariasql1 \
    --db-password=Placeholder1234 \
    --admin-firstname=John \
    --admin-lastname=Doe \
    --admin-email=johndoe@universe.com \
    --admin-user=johndoe@universe.com \
    --admin-password=Placeholder1234 \
    --language=de_DE \
    --currency=EUR \
    --timezone=Europe/Berlin \
    --use-rewrites=1 \
    --backend-frontname=admin \
    --cleanup-database

change mage enviroment to developer

    php bin/magento deploy:mode:set developer

add SampleData (only in Dev-Mode!)

    bin/magento sampledata:deploy

change mage admin url (optional)

    php bin/magento setup:config:set --backend-frontname="findme"

disable modules for build frontend

    php bin/magento module:disable Magento_TwoFactorAuth Magento_Csp

add frontools

    composer require snowdog/frontools
    composer require snowdog/module-alpaca-packages

optional

    php bin/magento maintenance:enable
    php bin/magento setup:upgrade
    php bin/magento setup:di:compile
    php bin/magento maintenance:disable

switch to frontools path & install yarn

    cd vendor/snowdog/frontools
    yarn install


optional step for broken stream().function

    yarn remove browser-sync
    yarn add browser-sync@2.18.12
    yarn setup
    cd dev/tools/frontools/config

edit config for Frontools

1. browser-sync.json
```
[
  {
    "proxy": "https://commerce.dev.lan",
    "open": false
  }
]
```
2. themes.json
```
{
  "alpaca": {
    "src": "vendor/snowdog/theme-frontend-alpaca",
    "dest": "pub/static/frontend/Snowdog/alpaca",
    "locale": ["de_DE"],
    "ignore": [
      "**/node_modules/**",
      "**/Snowdog_Components/docs/**",
      "**/Snowdog_Components/build/**"
    ]
  }
}
```

    cd tools
    yarn clean && yarn styles && yarn babel && yarn svg
    yarn dev

add github repositories

```
"repositories": [
        {
            "type": "vcs",
            "url":  "git@github.com:sickdaflip/mage2-foundation.git"
        },
        {
            "type": "vcs",
            "url":  "git@github.com:sickdaflip/mage2-foundation-frontools.git"
        }
    ]
```
> composer require flipdev/foundation dev-main

> composer require flipdev/module-foundation-frontools dev-main



