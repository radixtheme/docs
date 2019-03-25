# Radix 4.x
Documentation for Radix 4.x theme for Drupal 8.

## Requirements

1. [npm](https://www.npmjs.com) - [Read a guide on how to install Node and npm here](https://docs.npmjs.com/getting-started/installing-node).
2. [Drush](http://drush.org) - [Read a guide on how to install Drush here](http://www.drush.org/en/master/install/).
3. [Components module](https://www.drupal.org/project/components)

## Quick start for Drupal 8

1. Download and enable radix: `drush dl radix; drush en radix -y;`.
2. Create a subtheme: `drush radix "SUBTHEME NAME"`.
3. Set default theme: `drush en SUBTHEME_NAME -y; drush config-set system.theme default SUBTHEME_NAME -y`.
4. Install required modules: `cd /path/to/SUBTHEME_NAME; npm install;`.
5. Update proxy in `/path/to/SUBTHEME_NAME/webpack.mix.js`.
6. Watch: `npm run watch`.

## Using Composer
Use the following command to install Radix using composer. This will pull in Radix and the Components module.

```
composer require drupal/radix
```

# Support

1. Create an issue on [drupal.org](https://www.drupal.org/project/issues/radix).
2. Ask us on Twitter: [@radixtheme](http://twitter.com/radixtheme).
