# Ethnic_Food_Restaurant
This project was done as part of my CS6314 Web Programming Languages course

## Project Description:
1. Implemented a UI where a user can log in, view, and place orders for food items.
2. The user can also search for food items by any of the categories, price, name, and add them to their cart.
3. Also provided the admin functionalities where the administrator can log in with an authorized account and can insert, update, or delete the food items.

## Database Design:
The following collections were created:<br />                                                                                  1. Users: This collection is used to store information about all the registered users. It consists of the following fields:
  1.1 name: Stores the name of the user
  1.2 email: Stores the email id of the user
  1.3 phnno: Stores the phone number of the user
  1.4 password: Stores the hashed password of the user
  1.5 isAdmin: Stores boolean value to indicate whether a user is admin or not.
  1.6 currentToken: Stores the current authentication token of the user if is logged in otherwise stores null.
  
2. Products: This collection is used to store information about all the products available in the restaurant. It consists of the following fields:
  2.1 productName: Stores the name of the product.
  2.2 description: Stores the description of the product.
  2.3 category: Stores information about the category to which the product belongs. 
  2.4. price: Stores the price of the product.
  2.5. qty: Stores the quantity of product available in the inventory.
  2.6 image: Stores the image of the product
  2.7 isDeleted: This field is used to implement soft-delete.
  
3. Orders: This collection is used to store all the orders placed by the users. It consists of the following fields:
  3.1 CustomerID: It is used to identify the user who placed the order.
  3.2 Items: It consists of the array of information about the items placed as the order.
  3.3 orderType: This field specifies whether the user wants to place the order for dine-in or
  pick-up.
  3.4 bookingTime: stores the time at which order was placed.
  3.5 totalBill: stores the total amount of the order
  
## Languages/frameworks:
The following languages/frameworks were used in the project:

Front-end: HTML, CSS, JavaScript, React.js 
Back-end: Node.js, Express.js
Database: MongoDB