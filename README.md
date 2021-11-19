# magento-2-patches

## hawksearch_connector_2.4_magento_2.3.0-2.3.4-p2_compatibility_patch_cli 

HawkSearch_Connector extension version 2.4.* uses Laminas library which isn't supported by Magento below 2.3.5 version. For the purpose of providing new updates for customers who have Magento stores on versions 2.3.0-2.3.4-p2 Magento store owners need to install "hawksearch_connector_2.4_magento_2.3.0-2.3.4-p2_compatibility_patch_cli.patch"

Since "hawksearch/connector" composer package of version 2.4.* doesn't support Magento 2.3.0-2.3.4 it is not possible to use composer installation for HawkSearch extension package on that Magento version. Please install HawkSearch extension package from via files in `app/code` folder and then apply the patch.

### How to apply patch

Download the [patch file](https://raw.githubusercontent.com/hawksearch/magento-2-patches/main/hawksearch_connector_2.4_magento_2.3.0-2.3.4-p2_compatibility_patch_cli.patch) and apply it using one of commands bellow

```
patch -p1 < hawksearch_connector_2.4_magento_2.3.0-2.3.4-p2_compatibility_patch_cli.patch
```
```
git apply hawksearch_connector_2.4_magento_2.3.0-2.3.4-p2_compatibility_patch_cli.patch
```


Read more about [applying patches](https://devdocs.magento.com/guides/v2.3/comp-mgr/patching/command-line.html)


