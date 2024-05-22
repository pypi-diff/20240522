# Comparing `tmp/airbyte_source_shopify-2.1.0.dev202405090807.tar.gz` & `tmp/airbyte_source_shopify-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.1.0.dev202405090807.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.1.1.tar", max compression
```

## Comparing `airbyte_source_shopify-2.1.0.dev202405090807.tar` & `airbyte_source_shopify-2.1.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     4529 2024-05-09 08:01:04.344695 airbyte_source_shopify-2.1.0.dev202405090807/README.md
--rw-r--r--   0        0        0      816 2024-05-09 08:07:22.911137 airbyte_source_shopify-2.1.0.dev202405090807/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/run.py
--rw-r--r--   0        0        0    28417 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     2548 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     2135 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     2151 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0     1889 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0     1173 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     2162 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     3100 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     2628 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      986 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0    10233 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0     1621 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0     1775 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    24211 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     9939 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    23930 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     2042 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0     1114 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     2806 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0     1919 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0     1881 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0     1925 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0     1957 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0     2008 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0     1800 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0     1874 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0     1985 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0     1782 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0     1919 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0     2078 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0     1873 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0     1985 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    26296 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0     1549 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0   103922 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     2093 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     7004 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0     1760 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     4886 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0    13110 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     3598 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     8137 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0     2009 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0     2006 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     6603 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/scopes.py
--rw-r--r--   0        0        0        0 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/__init__.py
--rw-r--r--   0        0        0     1813 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    20409 2024-05-09 08:01:04.348695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    74083 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6517 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     1727 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/retry.py
--rw-r--r--   0        0        0      328 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/status.py
--rw-r--r--   0        0        0     3629 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-05-09 08:01:04.352695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-05-09 08:01:04.356695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8540 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/spec.json
--rw-r--r--   0        0        0    37215 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11754 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/transform.py
--rw-r--r--   0        0        0    13468 2024-05-09 08:01:04.360695 airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/utils.py
--rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.1.0.dev202405090807/PKG-INFO
+-rw-r--r--   0        0        0     4529 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/README.md
+-rw-r--r--   0        0        0      800 2024-05-22 19:57:02.553799 airbyte_source_shopify-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/run.py
+-rw-r--r--   0        0        0    28417 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     2548 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     2135 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     2151 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0     1889 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0     1173 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     2162 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     3100 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     2628 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      986 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0    10233 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0     1621 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0     1775 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    24211 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     9939 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    23930 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     2042 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0     1114 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     2806 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0     1919 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0     1881 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0     1925 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0     1957 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0     2008 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0     1800 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0     1874 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0     1985 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0     1782 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0     1919 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0     2078 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0     1873 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0     1985 2024-05-22 19:52:39.833201 airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    26296 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0     1549 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0   103922 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     2093 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     7004 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0     1760 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     4886 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0    13110 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     3598 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     8137 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0     2009 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0     2006 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     6603 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/scopes.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/__init__.py
+-rw-r--r--   0        0        0     1813 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    20372 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    74527 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6479 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     1704 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/retry.py
+-rw-r--r--   0        0        0      328 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/status.py
+-rw-r--r--   0        0        0     3629 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-05-22 19:52:39.837201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8518 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/spec.json
+-rw-r--r--   0        0        0    37215 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11754 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/transform.py
+-rw-r--r--   0        0        0    13468 2024-05-22 19:52:39.845201 airbyte_source_shopify-2.1.1/source_shopify/utils.py
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.1.1/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/README.md` & `airbyte_source_shopify-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/pyproject.toml` & `airbyte_source_shopify-2.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.1.0.dev202405090807"
+version = "2.1.1"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/__init__.py` & `airbyte_source_shopify-2.1.1/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/auth.py` & `airbyte_source_shopify-2.1.1/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.1.1/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customer_saved_search.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/customer_saved_search.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.1.1/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/scopes.py` & `airbyte_source_shopify-2.1.1/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from time import sleep, time
 from typing import Any, Final, Iterable, List, Mapping, Optional
 
 import pendulum as pdm
 import requests
-from airbyte_cdk import AirbyteLogger
 from requests.exceptions import JSONDecodeError
 from source_shopify.utils import ApiTypeEnum
 from source_shopify.utils import ShopifyRateLimiter as limiter
 
 from .exceptions import AirbyteTracedException, ShopifyBulkExceptions
 from .query import ShopifyBulkTemplates
 from .retry import bulk_retry_on_exception
@@ -25,15 +24,15 @@
 @dataclass
 class ShopifyBulkManager:
     session: requests.Session
     base_url: str
     stream_name: str
 
     # default logger
-    logger: Final[AirbyteLogger] = logging.getLogger("airbyte")
+    logger: Final[logging.Logger] = logging.getLogger("airbyte")
 
     # 10Mb chunk size to save the file
     _retrieve_chunk_size: Final[int] = 1024 * 1024 * 10
     _job_max_retries: Final[int] = 6
     _job_backoff_time: int = 5
     # saved latest request
     _request: Optional[requests.Request] = None
```

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1944,35 +1944,43 @@
             item["compareAtPrice"]["amount"] = float(compare_at_price_amount) if compare_at_price_amount else None
             item["compare_at_price"] = self.tools.fields_names_to_snake_case(item["compareAtPrice"])
             # remove leftovers
             item.pop("compareAtPrice", None)
 
         return entity
 
+    def _unnest_and_resolve_id(self, record: MutableMapping[str, Any], from_property: str, id_field: str) -> int:
+        entity = record.get(from_property, {})
+        return self.tools.resolve_str_id(entity.get(id_field)) if entity else None
+
     def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
         """
         Defines how to process collected components.
         """
 
         # get the joined record components collected for the record
         record_components = record.get("record_components", {})
         # process record components
         if record_components:
             record["presentment_prices"] = self._process_presentment_prices(record_components.get("ProductVariantPricePair", []))
             record.pop("record_components")
 
         # unnest mandatory fields from their placeholders
-        record["product_id"] = self.tools.resolve_str_id(record.get("product", {}).get("product_id"))
+        record["product_id"] = self._unnest_and_resolve_id(record, "product", "product_id")
+        record["inventory_item_id"] = self._unnest_and_resolve_id(record, "inventoryItem", "inventory_item_id")
+        record["image_id"] = self._unnest_and_resolve_id(record, "image", "image_id")
+        # unnest `fulfillment_service` from `fulfillmentService`
         record["fulfillment_service"] = record.get("fulfillmentService", {}).get("fulfillment_service")
-        record["inventory_item_id"] = self.tools.resolve_str_id(record.get("inventoryItem", {}).get("inventory_item_id"))
-        record["grams"] = int(record.get("grams", 0))
-        # cast the the `price` to number, could be literally `None`
+        # cast the `price` to number, could be literally `None`
         price = record.get("price")
         record["price"] = float(price) if price else None
+        # cast the `grams` to integer
+        record["grams"] = int(record.get("grams", 0))
         # convert date-time cursors
         record["createdAt"] = self.tools.from_iso8601_to_rfc3339(record, "createdAt")
         record["updatedAt"] = self.tools.from_iso8601_to_rfc3339(record, "updatedAt")
         # clean up the leftovers
+        record.pop("image", None)
         record.pop("product", None)
         record.pop("inventoryItem", None)
 
         yield record
```

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 import logging
 from dataclasses import dataclass, field
 from io import TextIOWrapper
 from json import loads
 from os import remove
 from typing import Any, Callable, Final, Iterable, List, Mapping, MutableMapping, Optional, Union
 
-from airbyte_cdk import AirbyteLogger
-
 from .exceptions import ShopifyBulkExceptions
 from .query import ShopifyBulkQuery
 from .tools import END_OF_FILE, BulkTools
 
 
 @dataclass
 class ShopifyBulkRecord:
     query: ShopifyBulkQuery
 
     # default buffer
     buffer: List[MutableMapping[str, Any]] = field(init=False, default_factory=list)
 
     # default logger
-    logger: Final[AirbyteLogger] = logging.getLogger("airbyte")
+    logger: Final[logging.Logger] = logging.getLogger("airbyte")
 
     def __post_init__(self) -> None:
         self.composition: Optional[Mapping[str, Any]] = self.query.record_composition
         self.record_process_components: Optional[Callable[[MutableMapping], MutableMapping]] = self.query.record_process_components
         self.components: List[str] = self.composition.get("record_components", []) if self.composition else []
 
     @property
```

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/retry.py` & `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/retry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Copyright (c) 2024 Airbyte, Inc., all rights reserved.
 
+import logging
 from functools import wraps
 from time import sleep
 from typing import Any, Callable, Final, Optional, Tuple, Type
 
-from airbyte_cdk import AirbyteLogger
-
 from .exceptions import ShopifyBulkExceptions
 
 BULK_RETRY_ERRORS: Final[Tuple] = (
     ShopifyBulkExceptions.BulkJobBadResponse,
     ShopifyBulkExceptions.BulkJobError,
 )
 
 
-def bulk_retry_on_exception(logger: AirbyteLogger, more_exceptions: Optional[Tuple[Type[Exception], ...]] = None) -> Callable:
+def bulk_retry_on_exception(logger: logging.Logger, more_exceptions: Optional[Tuple[Type[Exception], ...]] = None) -> Callable:
     """
     A decorator to retry a function when specified exceptions are raised.
 
     :param logger: Number of times to retry.
     :param more_exceptions: A tuple of exception types to catch.
     """
```

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.1.1/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/source.py` & `airbyte_source_shopify-2.1.1/source_shopify/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 
+import logging
 from typing import Any, List, Mapping, Tuple
 
-from airbyte_cdk import AirbyteLogger
 from airbyte_cdk.models import FailureType, SyncMode
 from airbyte_cdk.sources import AbstractSource
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.utils import AirbyteTracedException
 from requests.exceptions import ConnectionError, RequestException, SSLError
 
 from .auth import MissingAccessTokenError, ShopifyAuthenticator
@@ -139,15 +139,15 @@
         shop_name = config.get("shop")
         return shop_name.split(split_pattern)[0] if split_pattern in shop_name else shop_name
 
     @staticmethod
     def format_stream_name(name) -> str:
         return "".join(x.capitalize() for x in name.split("_"))
 
-    def check_connection(self, logger: AirbyteLogger, config: Mapping[str, Any]) -> Tuple[bool, any]:
+    def check_connection(self, logger: logging.Logger, config: Mapping[str, Any]) -> Tuple[bool, any]:
         """
         Testing connection availability for the connector.
         """
         config["shop"] = self.get_shop_name(config)
         config["authenticator"] = ShopifyAuthenticator(config)
         return ConnectionCheckTest(config).test_connection()
```

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/spec.json` & `airbyte_source_shopify-2.1.1/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.1.1/source_shopify/streams/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.1.1/source_shopify/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/transform.py` & `airbyte_source_shopify-2.1.1/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/source_shopify/utils.py` & `airbyte_source_shopify-2.1.1/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.0.dev202405090807/PKG-INFO` & `airbyte_source_shopify-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.1.0.dev202405090807
+Version: 2.1.1
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

