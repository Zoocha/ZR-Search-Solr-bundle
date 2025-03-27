# ZR Solr Search Recipe Installation Guide

To install the ZR Solr Search Recipe, follow the steps below:

1. Open your terminal.
2. Navigate to your project directory.
3. Add the below in the Drupal Root's composer.json installer-paths
```sh
"web/recipes/custom/{$name}": ["type:drupal-recipe"]
```
4. Run the following command to execute the ZR Solr Search Recipe installation:

    ```sh
    ddev drush recipe recipes/custom/solr-search-bundle
    ddev drush cim --partial --source=recipes/custom/solr-search-bundle/config -y

    ```

This command will execute the ZR Solr Search Recipe installation.
