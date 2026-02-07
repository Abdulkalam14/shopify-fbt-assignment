# Frequently Bought Together – Shopify Assignment

## Overview

This project implements a custom **Frequently Bought Together** feature inside the Shopify Dawn theme. The section allows store owners to select related products that appear on the product page. Customers can choose recommended items, see a live total price, and add all selected products to the cart in one click.

---

## Where the Code Was Added / Modified

The main implementation was added in:

**`sections/frequently-bought-together.liquid`**

This file contains:

* Liquid markup for rendering selected products
* JavaScript for dynamic total price calculation
* AJAX cart logic to add bundled products
* CSS styling for the user interface

No external apps or backend services were used. Everything was built directly inside the Shopify theme.

---

## How the Logic Works

1. The admin can select related products using Shopify’s product selection setting inside the section.

2. The selected products are displayed on the product page with a checkbox, image, title, and price.

3. When the user checks or unchecks products, JavaScript automatically updates the total price.

4. The main product price is always included in the total amount.

5. When the user clicks **Add Bundle to Cart**, all selected products are added to the cart together using Shopify’s cart system.

6. CSS is used to arrange everything in a clean grid layout with product cards and a bundle summary section.

---

## Assumptions / Notes

* For adding products to the cart, the first available variant of each product is used.

* This feature supports a simple bundle selection and does not include advanced variant customization.

* The layout is designed to match the Dawn theme and works properly on different screen sizes.

* The development store is password-protected as per Shopify’s default settings.

---

## Sources of Inspiration

The following resources helped in understanding Shopify theme customization:

* YouTube tutorials on Shopify custom sections and theme development
* This video was especially helpful:
  [https://www.youtube.com/watch?v=nJMqRgKkkBg](https://www.youtube.com/watch?v=nJMqRgKkkBg)

These resources were used only for learning setup concepts and implementation ideas.

---

## Result

The final implementation provides:

* A dynamic Frequently Bought Together section
* Live price calculation
* Bundle add-to-cart functionality
* Clean and modern UI styling

This solution works fully inside the Shopify Dawn theme without using any third-party apps.
