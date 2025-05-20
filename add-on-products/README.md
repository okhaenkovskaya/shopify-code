#  Additional products for product page

  

https://screenshotsbucket.s3.amazonaws.com/2025-01-06T14%3A39%3A23.213Z11f354b6-db93-47dd-b079-5d992d099794.png

  

**Section for product block with description, price, title etc.**

1. Copy snippet files

2. Add schema to the main-product.liquid

product blocks:

    {
    
    "type": "additional",
    
    "name": "Additional products",
    
	    "settings": [
	    
		    {
		    
			    "type": "inline_richtext",
			    
			    "id": "heading",
			    
			    "default": "Additional products",
			    
			    "label": "Heading"
		    
		    }
	    
	    ]
    
    },

  

render:

    {%- when  'additional' -%}
    
	    {% render  'additional-products' product: product, heading: block.settings.heading %}

  

Additional products stored in metafields according to each product

*Simple version - add to cart button with title and price*

*Large version - products with image, title, price and variants(only one swatch level). Qty for each product - optional*
