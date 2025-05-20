# Simple bundle products

https://aws3.link/udPtMo

**Bundle for product block**

1. Copy snippet files

2. Add schema to the main-product.liquid

product blocks:

    {

    "type": "additional",

    "name": "Bundle products",

        "settings": [

    	    {

    		    "type": "inline_richtext",

    		    "id": "heading",

    		    "default": "Bundle products",

    		    "label": "Heading"

    	    }

        ]

    },

render:

    {%- when  'additional' -%}
    	{%  render 'bundler' product: product %}

This block of Liquid template code is used to display a list of bundled products on a Shopify store. Products can be added on metafield for each product. For best performance - create dedicated product template for rpoduct with list on bundle products.

Or we can always use it on the simple product page template (block has js which hide native product add to cart button when bundler is added)

!Budnle products has only wirst level of variants (size or color or something else etc)
!Bundle products by default has 1 qty, but we can upgrade some parts of js code for different qty by each bundle product

TODO: Bundler discount code, reduce price for each product OR show total bundle price with sale
