﻿# Shopping Cart Project
 
 https://shoping-cart-snowy.vercel.app/

This is a simple shopping cart web page built with HTML, Bootstrap, and JavaScript.

## Features

- Two products: iPhone 11 and iPhone 11 Silicone Case.
- Users can increase or decrease the quantity of each product.
- Users can remove products from the cart.
- The cart automatically updates the subtotal and total price as quantities change.
- No tax is calculated; the total is simply the sum of all product prices.

## How It Works

### HTML Structure

- The cart displays each product with its image, name, quantity controls (plus/minus buttons), price, and a remove button.
- At the bottom, the cart shows the subtotal and total price.

### JavaScript Logic

- **handleProductChange(product, isIncreasing):**
  - Called when the plus or minus button is clicked.
  - Increases or decreases the product count.
  - Updates the product's total price.
  - Calls `calculateTotal()` to update the cart totals.

- **calculateTotal():**
  - Gets the current quantities for each product.
  - Calculates the total price (no tax).
  - Updates the subtotal and total price in the UI.

- **getInputValue(product):**
  - Reads the current quantity for a given product from the input field.

### Removing Products

- Clicking the remove icon hides the product from the cart, sets its quantity to 0, and updates the totals.

## Customization

- You can add more products by duplicating the product HTML and updating the JavaScript logic.
- To add tax or other fees, modify the `calculateTotal()` function.

## Dependencies

- [Bootstrap 4](https://getbootstrap.com/)
- [Font Awesome](https://fontawesome.com/)
