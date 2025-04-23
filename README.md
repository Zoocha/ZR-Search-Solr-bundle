# ZR Solr Search Recipe Installation Guide

To install the ZR Solr Search Recipe, follow the steps below:

1. Ensure the below has been added to the `composer.json` **installer-paths**:
    ```sh
    "web/recipes/custom/{$name}": ["type:drupal-recipe"]
    ```
2. Run `composer require zr/solr-search-bundle`
3. Run the following command (within `/web` directory):

    ```sh
    ddev drush recipe recipes/custom/solr-search-bundle
    ddev drush cim --partial --source=recipes/custom/solr-search-bundle/config -y
    ```
