# Data Model Questions

Some questions you might ask during the exercise:

1. What classes they would define.
1. What methods go in each class (including signatures).
1. What the class constructors are responsible for.
1. What data structures the class will have to maintain.
1. Whether any Design Patterns are applicable to this problem. 

## SaaS App

You are building a task management / productivity app where users can
add tasks and wireframes, and comment on both.  The scenario is:

* Tasks are a part of projects
* Projects are a part of customer accounts
* Users can be invited to several projects, in any customer account
* Some users can administer projects (add other users etc...), while others can only work in the project
* Each customer account can be managed by one or more users

## Hospital

You are building medical appointment software.  The software does the following:  

* Patients schedule meetings with doctors
* Doctors work in sometimes 1, sometimes 2 or 3 hospitals
* All doctors and patients need to be able to login
* There's a master list of all medications
* Doctors prescribe medications for patients

How would you model this?

## Social network

You are building a social network.  The software does the following:

* People can request friends, and friends can accept or deny  
* Users can post status updates
* Users can upload photos and manage photo albums
* Users can comment on posts
* Users can comment on photos
* Users can like posts, comments and photos
* Users can view all of their activity on the website

## Deck of cards

Design a deck of cards that can be used for different card game applications.

Likely classes: 
* a Deck
* a Card
* a Hand
* a Board
* Rank / Suit. 

Drill down on who's responsible for creating new Decks, where they get shuffled, how you deal cards, etc. 

Questions:

* Do you need a different instance for every card in a casino in Vegas?

## FileSystem

Create a class design to represent a filesystem.

Things like:

* Filesystem
* Directory
* File
* Permission 

Questions could be:

* What's their relationship? 
* How do you differentiate between text and binary files, or do you need to? 
* What about executable files? How do they model a Directory containing many files? 
* Do they use a data structure for it? Which one, and what performance tradeoffs does it have?

## HTML

Design an OO representation to model HTML.

* Nodes
* Attributes
* Children and parent pointers

The following commonly-asked OO design interview questions are probably too involved to be good phone-screen weeders:

   1. Design a parking garage.
   2. Design a bank of elevators in a skyscraper.
   3. Model the monorail system at Disney World.
   4. Design a restaurant-reservation system.
   5. Design a hotel room-reservation system. 

## SurveyMonkey / Google Forms

You are designing a tool that allows users to create surveys to send to other users.

* Admins can design surveys, with questions of the following types:
    * text field questions
    * dropdown questions that require a single answer
    * multiselect questions that allow users to select multiple answers
    * date questions
    * date range questions
    * numeric questions
    * single checkbox questions 
    * checkbox list questions that allow users to select multiple boxes
    * Likert scale questions 
* Some questions depend on the answers to other questions
    * For example: "if a user answers yes to this question, show these other two questions"
* Anonymous users can take surveys
* Logged in users can take surveys

Admins should be able to quickly answer questions like:

* How many users selected option A and option C from a multiselect question?
* How many people answered a date range question where their start date / end date includes 2014-05-04?
* What was the average of all of the answers to a numeric question?

## In-app messaging system

* Users can send messages to one or more other users
* Other users can reply to that thread
* Users can add other users to the conversation, or remove users

## CRM

You are building a CRM.  It tracks people and organizations.

* Users can manage people
* Users can manage organizations
* Users can create relationships between people (friend of, employer of etc...)
* Users can create relationships between people and organizations
* Some relationships between people and organizations need extra data - _for example_:
   * users should be able to define an "employment" relationship type, that has job title, start / end dates
   * users should be able to define a "volunteer" relationships type, which has things like t-shirt size or location
* Users can create relationships between organizations (for example if organizations have chapters, or different offices)
* Users can comment on both people and organizations
* Users can add multiple addresses, emails and phone numbers to both people and organizations

_can_ cover:

* polymorphic associations
* self-referential joins
* 

Some questions are things like:

* Single tenant or multi-tenant app
* Are the org / chapter relationships hierarchical or more of a graph?
* For the org / person relationships, hstore or fully modeled out?

## Apartment Rentals

TODO: Come up with an exercise that's like subscriptions:

* Time-based
* Units / people who fill units for a certain amount of time at a certain rate
* Have things like maintenance logs, account for when it was empty

## Airline Analytics

Imagine you run an airline.  You want to see how much money you have in profit in the air at any given point.

You want to see a map, where airplanes appear as lines on the map from one city to another, and on each line you see three numbers: income, expense and net for the flight.

## Model a card game, like Go fish

## Model a sports team

Include things like:

* Coaches
* Players

## Model a public elementary school

* Teachers
* Students
* Classrooms
* The classes that run in the classrooms at a given time

## Model a restaurant

* Tables
* Servers
* Reservations

## Model an apartment building:

```
Users want to be able to see a list of the apartments on all floors
Users want to be able to see details about an apartment, such as # of bedrooms, # of bathrooms and square footage
Users want to be able to see which apartments are vacant
Users want to be able to see a list of all tenants listed on every lease (current and previous) for an apartment
Users want to be able to see a list of rent checks, when they were received and deposited, for which leases
Users want to be able to see how much each apartment has made
Users want to be able to see the total amount of money they've taken in for a given lease
```
