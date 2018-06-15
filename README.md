# What is this?
This is a drop in replacement for the default product template in Shopify's Debut theme (though I'm sure the basic logic I've used could generally be applied to just about any theme.)

Basically it turns this:
![Default Color Dropdown](https://github.com/bryanchapel/shopify-debut-color-swatches/blob/master/screenshots/before.png "Default Color Dropdown")

Into this:
![New Color Swatches](https://github.com/bryanchapel/shopify-debut-color-swatches/blob/master/screenshots/after.png "New Color Swatches")

I actually like this approach because it utilizes assets already being included on the page, and since you're using a chunk of the actual product image, the swatch is very representative of the color (instead of trying to find the best match with a hex code). In some instances, like in the bag pic below, I thought the effect worked well by both highlighting the bag color as well as the text color in the swatch:

![Bag Color Swatches](https://github.com/bryanchapel/shopify-debut-color-swatches/blob/master/screenshots/bag.png "Bag Color Swatches")

# Usage:
1. Copy the contents from the `product-template.liquid` file to your own `product-template.liquid` file.
2. When using Color options during product creation, you can name the option type as either 'Color' or 'Colors', this should work for both.
3. The swatch is generated by taking the product image you link with the variant, blowing it up, and grabbing a 50x50px square area from the center of the image, which (for a centrally positioned clothing item at least) is typically a chunk of that item's color. You can play around with this, but that's the basic functionality out of the box.

That should be it! Both the styling for the swatches and the onclick `colorSwatchHandler()` function are located within this same template file for simplicity. So hack away!