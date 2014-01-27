shoppingBasketReceipt
=====================

Shopping Basket Receipt

Objective:
Create a program to generate a receipt for a shopping cart.

Given:
The input to the program includes: product description, product price, product quantity and location of the purchase. All other information, such as tax rates and product categories, is not part of the input and can be stored within the program or as part of configuration settings.
The program should calculate sales tax based on the location of the customer (consider only US states) and product category. Tax is calculated based on subtotal and should be rounded up to the nearest 0.05 (e.g. 1.13->1.15, 1.16->1.20)

Output
Program should generate a receipt with all items purchased and include description, price and quantity.

Tax rates
In California (CA), sales tax is applicable at a rate of 9.75% on all goods except food.
In New Jersey (NJ), general sales tax rate is 7.00%, food and clothing are exempt.

Unit Tests:
Input: Location: CA, 1-book-12.99, 1-potato chips-3.99	
Receipt:
           item          price            qty
           book         $12.99              1
   potato chips          $3.99              1
      subtotal:                        $16.98
           tax:                          $1.3
         total:                        $18.28

Input: Location: NJ, 1-book-12.99, 3-music cd-9.99
Receipt:
           item          price            qty
           book         $12.99              1
       music cd          $9.99              3
      subtotal:                        $42.96
           tax:                         $3.05
         total:                        $46.01


Input: Location: NJ, 2-music cd-9.99, 1-sweater-29.99
Receipt:
           item          price            qty
       music cd          $9.99              2
        sweater         $29.99              1
      subtotal:                        $49.97
           tax:                          $1.4
         total:                        $51.37
