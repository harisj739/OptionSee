# OptionSee

## Description
**Overview:**
Our group created a web application that allows users to search for and book flights. Users can login, create accounts, edit accounts, view past booking history, search for flights, pick a date and time for a flight, book ticket(s) for a flight, checkout a ticket, and logout. 

**Web Application Features:**
1. _**User Login:**_ A login page that requires users to enter their username and password. If found, the user is redirected to the home page. If not found, an error message tells the user that the account does not exist.
2. _**User Registration:**_ An account creation page where users can enter a new username and password in order to register an account. They are also required to enter user profile information as well, such as first name, last name, date of birth, sex, email, and phone. There is also a functionality that checks if the desired username is taken already. Once the account is created, the user is redirected to the home page.
3. _**Home:**_ The home page enables users to search for a flight based on location and departure date. When a location is selected from the dropdown, the user is redirected to a new page where they can select departure time and number of tickets.
4. _**Checkout:**_ Users can confirm flight and ticket information and then confirm their purchase of the ticket(s). Purchases are then added to the list of user’s previous bookings.
5. _**User Profile:**_ After registering, each user is able to view a separate page with their profile information and booking history.
6. _**User’s Completed Bookings:**_ After completing a booking, the user is able to find a list of their previous bookings on the “booking history” tab of their profile

**Form Element Implementation:**
We implemented text boxes, a drop down, radio buttons, and more as form elements. The text box was used for the search bar, a drop down was used for available flight locations, and a radio button to select a departure time for a flight.

**Database Implementation:** We created tables to store *airlines, airports, flights, locations, temptickets, tickets, and user info. 

**Team Collaboration:** We shared a Replit link and invited each other to work on the project. We also held multiple meetings to sync up and give updates.

**API Information:** We used local APIs for the users, flights, and bookings. The user API is accessed when looking up user profile information. The bookings API is accessed when looking up the user’s previous purchases.


## Task Distribution 
**Overview:**
We took on a more balanced approach throughout the team. Each of us took on a certain functionality of the website (i.e. login page, results page, user profile, etc.) and worked collaboratively on each of our parts.

**Primary Roles:**
1. Front-end layout and design, views: _Sukhdeep Kaur_
2. Back-end development, index.js, packages: _Haris Jilani_
3. Database management: _Andrew Grant_
4. Functionalities and interactivity: _Anthony Matricia_


## Changes from Original Design 

1. A temporary ticket was introduced to collect information about the flight being purchased by the user. When the user checks out, the information from the temporary ticket is copied into an official ticket table where it can later be accessed using the bookings API.
2. The database tables “flight” and “ticket” were modified to better suit their purposes. Originally, all the flight information was being saved in the “ticket” database table. However, this information would become repetitive as the flight information would repeat for each ticket. To avoid the clutter, we moved the flight information to “flight”, removing the ticketId to “flight”  and adding the flightId in “ticket”.
3. Originally we planned to use a flight tracker API to grab live flight bookings. However, we ended up using local API’s and populated them with our own flights. All our four API’s ended up being locally created API’s.

