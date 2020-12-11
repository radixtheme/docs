# Radix 4.x
Documentation for Radix 4.x theme for Drupal 8 and 9.

## Requirements

1. [npm](https://www.npmjs.com) - [Read a guide on how to install Node and npm here](https://docs.npmjs.com/getting-started/installing-node).
2. [Drush 8](http://drush.org) - [Read a guide on how to install Drush here](http://www.drush.org/en/master/install/).
3. [Components module](https://www.drupal.org/project/components)

## Quick start for Drupal 9 (with Drush 10)

1. Download and enable components 2.x: `composer require 'drupal/components:^2.0@beta'; drush en components -y`
2. Download and enable radix: `composer require 'drupal/radix'; drush theme:enable radix -y`
3. Clear caches: `drush cache-rebuild`
4. Create a subtheme: `drush --include=themes/contrib/radix radix:create SUBTHEME_NAME`
5. Enable the new theme: `drush theme:enable SUBTHEME_NAME -y`
6. Make it the default: `drush config-set system.theme default SUBTHEME_NAME -y`
7. Install required node modules: `cd themes/custom/SUBTHEME_NAME; npm install;`
8. Update the proxy URL in `themes/custom/SUBTHEME_NAME/webpack.mix.js`
9. Compile theme for development: `npm run dev`
10. Auto-compile changes: `npm run watch`

If drush reports 'There are no commands defined in the "radix" namespace.' for the `radix:create` command, then make sure you are running drush from the web root (i.e. the directory from which the inclue path `themes/contrib/radix` is valid).

## Quick start for Drupal 8

1. Download and enable radix: `composer require drupal/radix; drush en components radix -y`.
2. Create a subtheme: `drush --include="themes/contrib/radix" radix:create SUBTHEME NAME`.
3. Set default theme: `drush en SUBTHEME_NAME -y; drush config-set system.theme default SUBTHEME_NAME -y`.
4. Install required modules: `cd /path/to/SUBTHEME_NAME; npm install;`.
5. Update proxy in `/path/to/SUBTHEME_NAME/webpack.mix.js`.
6. Watch: `npm run watch`.

# Support

1. Create an issue on [drupal.org](https://www.drupal.org/project/issues/radix).
2. Ask us on Twitter: [@radixtheme](http://twitter.com/radixtheme).
