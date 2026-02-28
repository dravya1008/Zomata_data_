**Zomato Cart Recommendation System (Level-1)**  

This project simulates a food cart recommendation system similar to Zomato or food delivery apps.

When a user adds a food item to their cart, the system recommends additional items that are frequently ordered together.

**Example:**  

If a user adds "Pizza", the system may recommend:  

  
 • Garlic Bread  
 
 • Coke  
 
 • Pasta   
 
**Files** 

**orders.csv**

Contains order information

Example columns:

order_id → unique order number

user_id → customer id

order_number → order sequence of user

This tells which user placed which order.

**products.csv**

Contains product details

Example columns:

product_id

product_name

aisle_id

department_id

**order_products__prior.csv**

This is the most important file.

It tells which product was added in which order.


 
