# Products #

The products API allows you to view individual or a batch of products.

## Product attributes ##

| Attribute               | Type      | Description                                                                                                          |
|-------------------------|-----------|----------------------------------------------------------------------------------------------------------------------|
| `id`                    | integer   | Unique identifier for the product.                                                                                   |
| `name`                  | string    | Product name.                                                                                                        |
| `slug`                  | string    | Product slug.                                                                                                        |
| `permalink`             | string    | Product URL.                                                                                                         |
| `date_created`          | date-time | The date the product was created, in the site's timezone.                                                            |
| `date_created_gmt`      | date-time | The date the product was created, as GMT.                                                                            |
| `date_modified`         | date-time | The date the product was last modified, in the site's timezone.                                                      |
| `date_modified_gmt`     | date-time | The date the product was last modified, as GMT.                                                                      |
| `type`                  | string    | Product type. Options: `simple`, `grouped`, `external` and `variable`. Default is `simple`.                          |
| `featured`              | boolean   | Featured product. Default is `false`.                                                                                |
| `catalog_visibility`    | string    | Catalog visibility. Options: `visible`, `catalog`, `search` and `hidden`. Default is `visible`.                      |
| `description`           | string    | Product description.                                                                                                 |
| `short_description`     | string    | Product short description.                                                                                           |
| `sku`                   | string    | Unique identifier.                                                                                                   |
| `price`                 | string    | Current product price.                                                                                               |
| `regular_price`         | string    | Product regular price.                                                                                               |
| `sale_price`            | string    | Product sale price.                                                                                                  |
| `date_on_sale_from`     | date-time | Start date of sale price, in the site's timezone.                                                                    |
| `date_on_sale_from_gmt` | date-time | Start date of sale price, as GMT.                                                                                    |
| `date_on_sale_to`       | date-time | End date of sale price, in the site's timezone.                                                                      |
| `date_on_sale_to_gmt`   | date-time | End date of sale price, as GMT.                                                                                      |
| `on_sale`               | boolean   | Shows if the product is on sale.                                                                                     |
| `purchasable`           | boolean   | Shows if the product can be bought.                                                                                  |
| `total_sales`           | integer   | Amount of sales.                                                                                                     |
| `virtual`               | boolean   | If the product is virtual. Default is `false`.                                                                       |
| `downloadable`          | boolean   | If the product is downloadable. Default is `false`.                                                                  |
| `external_url`          | string    | Product external URL. Only for external products.                                                                    |
| `button_text`           | string    | Product external button text. Only for external products.                                                            |
| `manage_stock`          | boolean   | Stock management at product level. Default is `false`.                                                               |
| `stock_quantity`        | integer   | Stock quantity.                                                                                                      |
| `stock_status`          | string    | Controls the stock status of the product. Options: `instock`, `outofstock`, `onbackorder`. Default is `instock`.     |
| `backorders`            | string    | If managing stock, this controls if backorders are allowed. Options: `no`, `notify` and `yes`. Default is `no`.      |
| `backorders_allowed`    | boolean   | Shows if backorders are allowed.                                                                                     |
| `backordered`           | boolean   | Shows if the product is on backordered.                                                                              |
| `sold_individually`     | boolean   | Allow one item to be bought in a single order. Default is `false`.                                                   |
| `weight`                | string    | Product weight.                                                                                                      |
| `dimensions`            | object    | Product dimensions. See [Product - Dimensions properties](#product-dimensions-properties)                            |
| `shipping_required`     | boolean   | Shows if the product need to be shipped.                                                                             |
| `reviews_allowed`       | boolean   | Allow reviews.                                                                                                       |
| `average_rating`        | string    | Reviews average rating.                                                                                              |
| `rating_count`          | integer   | Amount of reviews that the product have.                                                                             |
| `reviews`               | array     | Returns product reviews if queried.                                                                                  |
| `review_count`          | integer   | Amount of reviews that the product have.                                                                             |
| `related_ids`           | array     | List of related products IDs.                                                                                        |
| `upsell_ids`            | array     | List of up-sell products IDs.                                                                                        |
| `cross_sell_ids`        | array     | List of cross-sell products IDs.                                                                                     |
| `parent_id`             | integer   | Product parent ID.                                                                                                   |
| `categories`            | array     | List of categories. See [Product - Categories properties](#product-categories-properties)                            |
| `tags`                  | array     | List of tags. See [Product - Tags properties](#product-tags-properties)                                              |
| `images`                | array     | List of images. See [Product - Images properties](#product-images-properties)                                        |
| `attributes`            | array     | List of attributes. See [Product - Attributes properties](#product-attributes-properties)                            |
| `default_attributes`    | array     | Defaults variation attributes. See [Product - Default attributes properties](#product-default-attributes-properties) |
| `variations`            | array     | List of variations IDs or details of each variation.                                                                 |
| `grouped_products`      | array     | List of grouped products ID.                                                                                         |
| `menu_order`            | integer   | Menu order, used to custom sort products.                                                                            |
| `meta_data`             | array     | Meta data. See [Product - Meta data properties](#product-meta-data-properties)                                       |

### Product - Dimensions properties ###

| Attribute | Type   | Description     |
|-----------|--------|-----------------|
| `length`  | string | Product length. |
| `width`   | string | Product width.  |
| `height`  | string | Product height. |

### Product - Categories properties ###

| Attribute | Type    | Description    |
|-----------|---------|----------------|
| `id`      | integer | Category ID.   |
| `name`    | string  | Category name. |
| `slug`    | string  | Category slug. |

### Product - Tags properties ###

| Attribute | Type    | Description |
|-----------|---------|-------------|
| `id`      | integer | Tag ID.     |
| `name`    | string  | Tag name.   |
| `slug`    | string  | Tag slug.   |

### Product - Images properties ###

| Attribute           | Type      | Description                                                   |
|---------------------|-----------|---------------------------------------------------------------|
| `id`                | integer   | Image ID.                                                     |
| `date_created`      | date-time | The date the image was created, in the site's timezone.       |
| `date_created_gmt`  | date-time | The date the image was created, as GMT.                       |
| `date_modified`     | date-time | The date the image was last modified, in the site's timezone. |
| `date_modified_gmt` | date-time | The date the image was last modified, as GMT.                 |
| `src`               | string    | Image URL.                                                    |
| `name`              | string    | Image name.                                                   |
| `alt`               | string    | Image alternative text.                                       |

### Product - Attributes properties ###

| Attribute   | Type    | Description                                                                                                       |
|-------------|---------|-------------------------------------------------------------------------------------------------------------------|
| `id`        | integer | Attribute ID.                                                                                                     |
| `name`      | string  | Attribute name.                                                                                                   |
| `position`  | integer | Attribute position.                                                                                               |
| `visible`   | boolean | Define if the attribute is visible on the "Additional information" tab in the product's page. Default is `false`. |
| `variation` | boolean | Define if the attribute can be used as variation. Default is `false`.                                             |
| `options`   | array   | List of available term names of the attribute.                                                                    |

### Product - Default attributes properties ###

| Attribute | Type    | Description                   |
|-----------|---------|-------------------------------|
| `id`      | integer | Attribute ID.                 |
| `name`    | string  | Attribute name.               |
| `option`  | string  | Selected attribute term name. |

### Product - Meta data properties ###

| Attribute | Type    | Description  |
|-----------|---------|--------------|
| `id`      | integer | Meta ID.     |
| `key`     | string  | Meta key.    |
| `value`   | string  | Meta value.  |

## Retrieve a product ##

This API lets you retrieve and view a specific product by ID.

### HTTP request ###

<div class="api-endpoint">
	<div class="endpoint-data">
		<i class="label label-get">GET</i>
		<h6>/wp-json/cocart/v1/products/&lt;id&gt;</h6>
	</div>
</div>

```shell
curl https://example.com/wp-json/cocart/v1/products/329 \
  -H "Content-Type: application/json" \
```

> JSON response example:

```json
{
  "id": 329,
  "name": "The Last of Us Part 2 - Ellie Edition",
  "slug": "the-last-of-us-part-2-ellie-edition",
  "permalink": "https://wp-demo.cocart.xyz/product/the-last-of-us-part-2-ellie-edition/",
  "date_created": "2020-02-12T17:01:46",
  "date_created_gmt": "2020-02-12T16:01:46",
  "date_modified": "2020-02-12T17:01:46",
  "date_modified_gmt": "2020-02-12T16:01:46",
  "type": "simple",
  "featured": false,
  "catalog_visibility": "visible",
  "description": "",
  "short_description": "",
  "sku": "",
  "price": "£180.00",
  "regular_price": "£180.00",
  "sale_price": "",
  "date_on_sale_from": null,
  "date_on_sale_from_gmt": null,
  "date_on_sale_to": null,
  "date_on_sale_to_gmt": null,
  "on_sale": false,
  "purchasable": true,
  "total_sales": 0,
  "virtual": false,
  "downloadable": false,
  "external_url": "",
  "button_text": "",
  "manage_stock": false,
  "stock_quantity": null,
  "in_stock": true,
  "stock_status": "instock",
  "backorders": "no",
  "backorders_allowed": false,
  "backordered": false,
  "sold_individually": false,
  "weight": "",
  "dimensions": {
    "length": "",
    "width": "",
    "height": ""
  },
  "shipping_required": true,
  "reviews_allowed": false,
  "average_rating": "0",
  "rating_count": 0,
  "review_count": 0,
  "rating_html": "",
  "reviews": [],
  "related_ids": [],
  "upsell_ids": [],
  "cross_sell_ids": [],
  "parent_id": 0,
  "categories": [
    {
      "id": 42,
      "name": "Video Games",
      "slug": "video-games"
    }
  ],
  "tags": [],
  "images": [
    {
      "id": 330,
      "date_created": "2020-02-12T18:00:39",
      "date_created_gmt": "2020-02-12T16:00:39",
      "date_modified": "2020-02-12T18:00:39",
      "date_modified_gmt": "2020-02-12T16:00:39",
      "src": {
        "thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-150x150.jpg",
        "medium": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-169x300.jpg",
        "medium_large": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-768x1365.jpg",
        "large": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-576x1024.jpg",
        "1536x1536": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-864x1536.jpg",
        "2048x2048": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A.jpg",
        "woocommerce_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-324x324.jpg",
        "woocommerce_single": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-416x740.jpg",
        "woocommerce_gallery_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-100x100.jpg",
        "shop_catalog": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-324x324.jpg",
        "shop_single": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-416x740.jpg",
        "shop_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-100x100.jpg",
        "full": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A.jpg",
        "custom": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A.jpg"
      },
      "name": "TLOU2_WP_DUALITY_1080X1920_002A",
      "alt": "",
      "position": 0
    }
  ],
  "attributes": [],
  "default_attributes": [],
  "variations": [],
  "grouped_products": [],
  "menu_order": 0,
  "meta_data": [],
  "yoast_seo_meta": {
    "title": null,
    "description": null,
    "focus_keyword": null,
    "content_score": null,
    "linkdex": null,
    "primary_product_category": null
  },
  "_links": {
    "self": [
      {
        "permalink": "https://wp-demo.cocart.xyz/product/the-last-of-us-part-2-ellie-edition/",
        "href": "https://wp-demo.cocart.xyz/wp-json/cocart/v1/products/329"
      }
    ],
    "collection": [
      {
        "permalink": "https://wp-demo.cocart.xyz/",
        "href": "https://wp-demo.cocart.xyz/wp-json/cocart/v1/products"
      }
    ]
  }
}
```

## List all products ##

This API helps you to view all the products.

### HTTP request ###

<div class="api-endpoint">
	<div class="endpoint-data">
		<i class="label label-get">GET</i>
		<h6>/wp-json/cocart/v1/products</h6>
	</div>
</div>

```shell
curl https://example.com/wp-json/cocart/v1/products \
  -H "Content-Type: application/json" \
```

> JSON response example:

```json
[
  {
    "id": 329,
    "name": "The Last of Us Part 2 - Ellie Edition",
    "slug": "the-last-of-us-part-2-ellie-edition",
    "permalink": "https://wp-demo.cocart.xyz/product/the-last-of-us-part-2-ellie-edition/",
    "date_created": "2020-02-12T17:01:46",
    "date_created_gmt": "2020-02-12T16:01:46",
    "date_modified": "2020-02-12T17:01:46",
    "date_modified_gmt": "2020-02-12T16:01:46",
    "type": "simple",
    "featured": false,
    "catalog_visibility": "visible",
    "description": "",
    "short_description": "",
    "sku": "",
    "price": "£180.00",
    "regular_price": "£180.00",
    "sale_price": "",
    "date_on_sale_from": null,
    "date_on_sale_from_gmt": null,
    "date_on_sale_to": null,
    "date_on_sale_to_gmt": null,
    "on_sale": false,
    "purchasable": true,
    "total_sales": 0,
    "virtual": false,
    "downloadable": false,
    "external_url": "",
    "button_text": "",
    "manage_stock": false,
    "stock_quantity": null,
    "in_stock": true,
    "stock_status": "instock",
    "backorders": "no",
    "backorders_allowed": false,
    "backordered": false,
    "sold_individually": false,
    "weight": "",
    "dimensions": {
      "length": "",
      "width": "",
      "height": ""
    },
    "shipping_required": true,
    "reviews_allowed": false,
    "average_rating": "0",
    "rating_count": 0,
    "review_count": 0,
    "rating_html": "",
    "reviews": [],
    "related_ids": [],
    "upsell_ids": [],
    "cross_sell_ids": [],
    "parent_id": 0,
    "categories": [
      {
        "id": 42,
        "name": "Video Games",
        "slug": "video-games"
      }
    ],
    "tags": [],
    "images": [
      {
        "id": 330,
        "date_created": "2020-02-12T18:00:39",
        "date_created_gmt": "2020-02-12T16:00:39",
        "date_modified": "2020-02-12T18:00:39",
        "date_modified_gmt": "2020-02-12T16:00:39",
        "src": {
          "thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-150x150.jpg",
          "medium": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-169x300.jpg",
          "medium_large": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-768x1365.jpg",
          "large": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-576x1024.jpg",
          "1536x1536": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-864x1536.jpg",
          "2048x2048": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A.jpg",
          "woocommerce_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-324x324.jpg",
          "woocommerce_single": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-416x740.jpg",
          "woocommerce_gallery_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-100x100.jpg",
          "shop_catalog": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-324x324.jpg",
          "shop_single": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-416x740.jpg",
          "shop_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A-100x100.jpg",
          "full": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A.jpg",
          "custom": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/02/TLOU2_WP_DUALITY_1080X1920_002A.jpg"
        },
        "name": "TLOU2_WP_DUALITY_1080X1920_002A",
        "alt": "",
        "position": 0
      }
    ],
    "attributes": [],
    "default_attributes": [],
    "variations": [],
    "grouped_products": [],
    "menu_order": 0,
    "meta_data": [],
    "yoast_seo_meta": {
      "title": null,
      "description": null,
      "focus_keyword": null,
      "content_score": null,
      "linkdex": null,
      "primary_product_category": null
    },
    "_links": {
      "self": [
        {
          "permalink": "https://wp-demo.cocart.xyz/product/the-last-of-us-part-2-ellie-edition/",
          "href": "https://wp-demo.cocart.xyz/wp-json/cocart/v1/products/329"
        }
      ],
      "collection": [
        {
          "permalink": "https://wp-demo.cocart.xyz/",
          "href": "https://wp-demo.cocart.xyz/wp-json/cocart/v1/products"
        }
      ]
    }
  },
  {
    "id": 185,
    "name": "WordPress Pennant",
    "slug": "wordpress-pennant",
    "permalink": "https://wp-demo.cocart.xyz/product/wordpress-pennant/",
    "date_created": "2020-01-24T14:55:56",
    "date_created_gmt": "2020-01-24T13:55:56",
    "date_modified": "2020-01-24T14:56:40",
    "date_modified_gmt": "2020-01-24T13:56:40",
    "type": "external",
    "featured": false,
    "catalog_visibility": "visible",
    "description": "Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum tortor quam, feugiat vitae, ultricies eget, tempor sit amet, ante. Donec eu libero sit amet quam egestas semper. Aenean ultricies mi vitae est. Mauris placerat eleifend leo.",
    "short_description": "This is an external product.",
    "sku": "wp-pennant",
    "price": "£11.05",
    "regular_price": "£11.05",
    "sale_price": "",
    "date_on_sale_from": null,
    "date_on_sale_from_gmt": null,
    "date_on_sale_to": null,
    "date_on_sale_to_gmt": null,
    "on_sale": false,
    "purchasable": false,
    "total_sales": 0,
    "virtual": false,
    "downloadable": false,
    "external_url": "https://mercantile.wordpress.org/product/wordpress-pennant/",
    "button_text": "Buy on the WordPress swag store!",
    "manage_stock": false,
    "stock_quantity": null,
    "in_stock": true,
    "stock_status": "instock",
    "backorders": "no",
    "backorders_allowed": false,
    "backordered": false,
    "sold_individually": false,
    "weight": "",
    "dimensions": {
      "length": "",
      "width": "",
      "height": ""
    },
    "shipping_required": true,
    "reviews_allowed": true,
    "average_rating": "0",
    "rating_count": 0,
    "review_count": 0,
    "rating_html": "",
    "reviews": [],
    "related_ids": [],
    "upsell_ids": [],
    "cross_sell_ids": [],
    "parent_id": 0,
    "categories": [
      {
        "id": 29,
        "name": "Decor",
        "slug": "decor"
      }
    ],
    "tags": [],
    "images": [
      {
        "id": 208,
        "date_created": "2020-01-24T15:56:39",
        "date_created_gmt": "2020-01-24T13:56:39",
        "date_modified": "2020-01-24T15:56:39",
        "date_modified_gmt": "2020-01-24T13:56:39",
        "src": {
          "thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-150x150.jpg",
          "medium": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-300x300.jpg",
          "medium_large": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-768x768.jpg",
          "large": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1.jpg",
          "1536x1536": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1.jpg",
          "2048x2048": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1.jpg",
          "woocommerce_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-324x324.jpg",
          "woocommerce_single": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-416x416.jpg",
          "woocommerce_gallery_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-100x100.jpg",
          "shop_catalog": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-324x324.jpg",
          "shop_single": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-416x416.jpg",
          "shop_thumbnail": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1-100x100.jpg",
          "full": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1.jpg",
          "custom": "https://wp-demo.cocart.xyz/wp-content/uploads/2020/01/pennant-1.jpg"
        },
        "name": "pennant-1.jpg",
        "alt": "",
        "position": 0
      }
    ],
    "attributes": [],
    "default_attributes": [],
    "variations": [],
    "grouped_products": [],
    "menu_order": 0,
    "meta_data": [],
    "yoast_seo_meta": {
      "title": null,
      "description": null,
      "focus_keyword": null,
      "content_score": null,
      "linkdex": null,
      "primary_product_category": null
    },
    "_links": {
      "self": [
        {
          "permalink": "https://wp-demo.cocart.xyz/product/wordpress-pennant/",
          "href": "https://wp-demo.cocart.xyz/wp-json/cocart/v1/products/185"
        }
      ],
      "collection": [
        {
          "permalink": "https://wp-demo.cocart.xyz/",
          "href": "https://wp-demo.cocart.xyz/wp-json/cocart/v1/products"
        }
      ]
    }
  }
]
```

#### Available parameters ####

| Parameter           | Type    | Description                                                                                                                                                    |
|---------------------|---------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `page`              | integer | Current page of the collection. Default is `1`.                                                                                                                |
| `per_page`          | integer | Maximum number of items to be returned in result set. Default is `10`.                                                                                         |
| `search`            | string  | Limit results to those matching a string.                                                                                                                      |
| `after`             | string  | Limit response to resources published after a given ISO8601 compliant date.                                                                                    |
| `before`            | string  | Limit response to resources published before a given ISO8601 compliant date.                                                                                   |
| `exclude`           | array   | Ensure result set excludes specific IDs.                                                                                                                       |
| `include`           | array   | Limit result set to specific ids.                                                                                                                              |
| `offset`            | integer | Offset the result set by a specific number of items.                                                                                                           |
| `order`             | string  | Order sort attribute ascending or descending. Options: `asc` and `desc`. Default is `desc`.                                                                    |
| `orderby`           | string  | Sort collection by object attribute. Options: `date`, `id`, `include`, `title` and `slug`. Default is `date`.                                                  |
| `parent`            | array   | Limit result set to those of particular parent IDs.                                                                                                            |
| `parent_exclude`    | array   | Limit result set to all items except those of a particular parent ID.                                                                                          |
| `slug`              | string  | Limit result set to products with a specific slug.                                                                                                             |
| `type`              | string  | Limit result set to products assigned a specific type. Options: `simple`, `grouped`, `external`, `variable`, `simple-subsciption` and `variable-subscription`. |
| `sku`               | string  | Limit result set to products with a specific SKU.                                                                                                              |
| `featured`          | boolean | Limit result set to featured products.                                                                                                                         |
| `category`          | string  | Limit result set to products assigned a specific category ID.                                                                                                  |
| `tag`               | string  | Limit result set to products assigned a specific tag ID.                                                                                                       |
| `attribute`         | string  | Limit result set to products with a specific attribute.                                                                                                        |
| `attribute_term`    | string  | Limit result set to products with a specific attribute term ID (required an assigned attribute).                                                               |
| `on_sale`           | boolean | Limit result set to products on sale.                                                                                                                          |
| `min_price`         | string  | Limit result set to products based on a minimum price.                                                                                                         |
| `max_price`         | string  | Limit result set to products based on a maximum price.                                                                                                         |
| `stock_status`      | string  | Limit result set to products with specified stock status. Options: `instock`, `outofstock` and `onbackorder`.                                                  |
| `show_reviews`      | boolean | Set to true to return product reviews.                                                                                                                         |
| `return_variations` | boolean | Set to true to return the variations of variable products.                                                                                                     |