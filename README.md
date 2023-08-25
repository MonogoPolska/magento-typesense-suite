# Typesense Magento integration

Set of packages for Magento 2 Typesense implementation

## Configuration
As the first step, Go to Magento Admin &rarr; Configuration &rarr; Typesense

### General section
Configure the connection parameters for Typesense instance

### Advanced section
Configure the additional parameters

### Indexing Queue / Cron section
Configure Queue/Cron for indexers

### Catalog Categories
Configure Catalog Categories

### CMS Pages
Configure Queue/Cron for indexers

### Analytics
Configure Analytics

## CLI

| Command                              | Description                                      |
|--------------------------------------|--------------------------------------------------|
| ```bin/magento typesense:compact```  | Compact the on-disk database of Typesense server |
| ```bin/magento typesense:flush```    | Flush all imported data in Typesense             |
| ```bin/magento typesense:metrics```  | Get Typesense server metrics                     |

## Indexers

| Indexer                                                  | Description                                                                                                                        |
|----------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
| ```bin/magento indexer:reindex typesense_queue_runner``` | Typesense Queue Runner. To enable this, configure <br/>Stores &rarr; Configuration &rarr;Typesense &rarr; Indexing Queue / Cron    |
| ```bin/magento indexer:reindex typesense_all```          | Metaindexer. It will runn all dependent indexes defined in modules                                                                 |
| ```bin/magento indexer:reindex typesense_categories```   | Typesense Categories indexer. To enable this, configure <br/>Stores &rarr; Configuration &rarr;Typesense &rarr; Catalog Categories |
| ```bin/magento indexer:reindex typesense_cms_pages```    | Typesense CMS Pages indexer. To enable this, configure <br/>Stores &rarr; Configuration &rarr;Typesense &rarr; CMS Pages           |


# Credits
- [Monogo](https://monogo.pl/en)
- [Typesense](https://typesense.org)
- [Official Algolia magento module](https://github.com/algolia/algoliasearch-magento-2)
