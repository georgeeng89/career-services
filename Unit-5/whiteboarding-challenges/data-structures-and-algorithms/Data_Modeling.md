# Data Modeling

## Suggested Process

1. Ask question and set up problem
1. Clarify any questions the interviewee has
1. Interviewee explains an answer either verbally or with a whiteboard
1. Give interviewee a chance to clarify anything you notice wrong or odd

## Questions and Answers

### Movies and Actors

#### Question

How would you model movies and actors?

#### Answer

One movie has many actors, and each actor is in many movies. If a proper join table is used (like "Appearance"), Actor will have a one-to-many with Appearance, which will have a many-to-one relationship with Actor.

### Library

#### Question

How would you model a library? Account for books, authors, and patrons. You should be able to tell which books are checked out by which patrons.

#### Answer

* Book has a many-to-many relationship with Author. This should have a joining table, like BookAuthor.
* Patron should have a many-to-many relationship with Book. This joining table is the checkout record.
* The CheckoutRecord shoud have the date the book was checked out, and a date returned. If there's a checkout date

### Sales & Inventory System

#### Question

How would you model a sales and inventory system? Account for products, product manufacturers, orders, shipments, payments, customers, and salespeople. Each order can have multiple forms of payment. Each order has one customer and one salesperson.

#### Answer

* One Supplier has many Products
* Each Product has many Orders, each Order has many Products. This should have a joining table, like ProductOrder.
* Each Salesman has many Orders
* Each Customer has many Customers
* Each Order has many Shipments
* Each Order has many Payments
* Look for appropriate fields in each table
