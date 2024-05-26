# Online shop

## Functional Requirements
### 1.User Registration and Authentication
+ Users can create accounts.
+ Users can log in and log out.

### 2.Product Management

+ Admins can add new products.
+ Admins can update existing product details.
+ Admins can delete products.
+ Users can view product details.
+ Users can search for products.
### 3.Shopping Cart

+ Users can add products to the shopping cart.
+ Users can view their cart contents.
+ Users can update quantities or remove items from the cart.
### 4.Checkout and Orders

+ Users can proceed to checkout from the shopping cart.
+ Users can view their order history.
+ Users receive email notifications on order placement and shipment.
### 5.Payment Integration

+ Users can pay for their orders using a payment gateway (e.g., Stripe, PayPal).
+ Payment information should be securely stored.
### 6.User Reviews and Ratings

+ Users can leave reviews and ratings for products.
+ Reviews and ratings can be viewed by all users.
### 7.User Profile

+ Users can edit their profiles.
+ Users can view their order history and track shipments.
### 8.Admin Panel

+ Admins can manage user accounts (ban, delete).
+ Admins can view and manage orders.
+ Admins can view sales reports.
### 9.Security and Privacy

+ User passwords should be stored securely (hashed and salted).
+ Payment information should be encrypted.
+ HTTPS should be used to protect data transmission.
### 10.Localization and Currency

+ The system should support multiple languages.
+ The system should support multiple currencies.
+ Currency conversion should be accurate and up-to-date.

## System Behaviors
### 1.User Registration and Authentication

Users can register with their email address and password.
Users can log in using their credentials.
Sessions should expire after a period of inactivity.
### 2.Product Management

Admins can add products with details such as name, description, price, and images.
Product details can be updated.
Products can be deleted.
### 3.Shopping Cart

Users can add products to the cart without logging in.
The cart should persist between sessions for logged-in users.
Users should be able to adjust quantities and remove items.
### 4.Checkout and Orders

Users must provide shipping information during checkout.
Orders should be recorded in the database.
Users should receive confirmation emails with order details.
### 5.Payment Integration

Payment gateway should handle transactions securely.
Users should receive a payment confirmation after completing the transaction.
### 6.User Reviews and Ratings

Reviews and ratings should be linked to specific products.
Users should be able to edit or delete their own reviews.
### 7.User Profile

Users can update their profile information.
Users can view their past orders and order statuses.
### 8.Admin Panel

Admins can access an administrative dashboard.
Admins can view sales reports for a selected time period.
Admins can manage user accounts and orders.
### 9.Security and Privacy

Passwords should be hashed with a strong hashing algorithm.
Payment information should be encrypted using industry-standard encryption protocols.
Data transmission should be secured using HTTPS.
### 10.Localization and Currency

Users should be able to select their preferred language.
Users should be able to view prices in their selected currency.
Currency conversion rates should be updated regularly.
