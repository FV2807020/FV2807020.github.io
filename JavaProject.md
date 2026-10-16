**Java Project**

This is a coding project using Java to test my understanding of the Fundementals of Java.

Step 1 — Brainstorm and plan

Write at least three different program ideas. Choose one and explain:

What will your program do?
Who might use it or enjoy it?
What information will the user enter?
What decisions will your program make?
Which variables and data types will you need?

FIIRST IDEAS:

**Resturant Reservation**
Task: Reserve Seats in a Restaurant for certain dates, up to months ahead.
User: Restaurant goers will use it
Information Entered: Dates, Times, Number of People Eg. Date: 4/4/26 Time: 4:30 - 5:00, Occupants: 5
Decisions made: decide wether to place in little tables (1-2), medium tables(3-5), or large tables (5+)
Variables and Data Types Needed: Strings to tell time and Booleans to confirm seats, tables, dates, times, etc.

**Parking Garage Spot Reserver System**
Task: Reserve Parking Spots for a busy convention center on certain dates for certain times
User: Everyday people
Information Entered: dates and times
Decisions made: is there parking? where should the person park
Variables and Data Types Needed: booleans

**Flight Booker System**
Task: Reserve seats on a flight
User: people who want to take flights
Information Entered: dates and times
Decisions made: is a seat taken? if not, reserve person to seat there
Variables and Data Types Needed: booleans

I chose the restaurant reservation system, to me it looks the most challenging and the most complex.

"C. Decompose the project

Break your project down into parts, example:
Beginning:
Welcome user
Give instructions
Take user input to set up program
Main program:
Decision to be made/game structure
Class instance variables/methods
Output/end:
Print recommendation/show update/end game
Plan each part, example:
Welcome user: print "Welcome to ______! Here, you will be able to ____"
Give instructions: "Please enter your name:" "Please enter your preference"
Decision to be made: "If user prefers beaches and wants to go somewhere exotic, and has a budget of at least $4000 per person, recommend Bora Bora or Maldives for their vacation""

MY INTERPRETATION
Beginning:
Welcome user: print "Welcome to *INSERT RESTURANT NAME*! Here, you will be able to reserve your seat"
1. Please Enter Your Name
2. Please Enter your Group Size
3. Please Enter the Date you want to Come


Main program:
1. Please Enter Your First and Last Name
  
3. Please Enter your Group Size
   if size = 0, display error (Group Size can not be 0!) and return to answer screen
   if size < 3, send to small couples tables
   if size >2, <6, send to small family tables
   if size >5, <11, send to big family / meeting tables
   if size >10, display error (You must reserve multiple tables for group sizes >11)
5. Please Enter the Date you want to Come, up to a month in advance


Output/end:





















