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

  **🍕 Zomato-Style Food Recommendation System**

Welcome to the tiny brain behind your late-night cravings 😋

Ever wondered why food apps magically suggest Coke with Pizza or Fries with Burger?
This project is a mini version of that recommendation system.

Think of it as a food-loving robot 🤖 that observes what people order and suggests extra tasty add-ons to increase the cart value.

🧠 What This Project Does

Imagine a user opening a food delivery app.

The system checks:

🏙 User City

⏰ Time of Order

🍽 Restaurant Type

🛒 Cart Size

🍕 Item Ordered

Then it recommends an add-on item.

Example:

User Order	Recommendation
Pizza	Coke
Burger	Fries
Biryani	Raita

Basically:

Pizza ➜ Coke
Burger ➜ Fries
Biryani ➜ Raita

Because food tastes better with friends (and by friends we mean side dishes 😌).

📊 Dataset

We created a synthetic dataset of 50 orders that mimics food delivery behaviour.

Example:

user_id	city	time	item	cart_size	recommendation  
user_1	Delhi	lunch	pizza	1	coke 

user_2	Mumbai	evening	burger	2	fries


⚙️ How the Recommendation Works

The system follows simple rules.

Rule 1: Item Based Recommendation
Pizza ➜ Coke
Burger ➜ Fries
Biryani ➜ Raita
Rule 2: Time Based Recommendation
Time	Suggested Item
Morning	Coffee
Lunch	Meals
Evening	Snacks
Night	Comfort food
Rule 3: Cart Size Logic
cart_size >= 3 ➜ Dessert

Because if you're already ordering a lot…
why not add dessert too? 🍰


**Input:**

City: Delhi
Time: Evening
Item Ordered: Pizza
Cart Size: 1

**Output:**

Recommended Item → Coke

The system basically says:

“Hey… you forgot the drink 🥤”

**🌍 Real World Inspiration**

Food delivery platforms like:

Zomato

Swiggy

use machine learning and massive datasets to recommend items.

This project is a simplified prototype showing the core logic behind such recommendation systems.

📈 Future Improvements

Things we could add next:

Market Basket Analysis (Apriori Algorithm)

Machine Learning recommendations

User history based recommendations

Restaurant popularity trends

🎯 Project Goal

The goal of this project is to demonstrate:

How recommendation systems work

How food delivery apps increase cart value

How user behaviour influences suggestions

All with just a tiny dataset and some clever logic.

🍔 Final Thought

If someone orders Pizza without Coke…

Our system politely whispers:

“Are you sure about that decision?” 😏  

**🆕 New User Recommendation (Cold Start Problem)**

When a new user logs in, the system has no order history to understand their preferences.

This is called the Cold Start Problem in recommendation systems.

Since the system doesn't know the user's taste yet, it recommends popular food combinations ordered by other users.

Food delivery platforms like Zomato often use this strategy to quickly engage new users.

**🍔 Recommendation Strategy**

The system follows a popularity-based recommendation approach.

Steps:

1️⃣ User logs into the platform
2️⃣ System checks if the user has previous orders
3️⃣ If no order history exists, the system selects the most popular food combos
4️⃣ Top combos are shown as recommendations

Example logic:

If user_history == empty:
    recommend top popular combos
📊 Dataset

The dataset contains synthetic food delivery order data used to identify popular combos.

Example:

City	Combo	Popularity
Delhi	Pizza + Coke	420
Mumbai	Burger + Fries	380
Bangalore	Dosa + Filter Coffee	300
**🧠 Recommendation Logic**

The system ranks combos using popularity score.

Example recommendations:

1️⃣ Pizza + Coke
2️⃣ Burger + Fries
3️⃣ Biryani + Raita

These combos are recommended to new users with no past order data.



 
