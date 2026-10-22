**Java Project** 
**Resturant Reservation System**

This is a coding project using Java to test my understanding of the Fundementals of Java.

**Step 1**
— Brainstorm and plan Write at least three different program ideas. 

Choose one and explain: What will your program do? Who might use it or enjoy it? What information will the user enter? What decisions will your program make? Which variables and data types will you need? 

FIIRST IDEAS: **Resturant Reservation** 
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

"C. Decompose the project Break your project down into parts, example: 
Beginning: Welcome user Give instructions Take user input to set up program 
Main program: Decision to be made/game structure Class instance variables/methods 
Output/end: Print recommendation/show update/end game Plan each part, 
example: Welcome user: print "Welcome to ______! Here, you will be able to ____" 
Give instructions: "Please enter your name:" "Please enter your preference" 
Decision to be made: "If user prefers beaches and wants to go somewhere exotic, and has a budget of at least $4000 per person, recommend Bora Bora or Maldives for their vacation"" 


MY INTERPRETATION 
Beginning: Welcome user: print "Welcome to *INSERT RESTURANT NAME*! Here, you will be able to reserve your seat"
1. Please Enter Your Name
 Please Enter your Group Size
 Please Enter the Date you want to Come
 Main program:
 (import time package)
 (import scanner package)
 1. Please Enter Your First and Last Name
 2.  Store in system if 7 success
 3.   Please Enter your Group Size In a Single Integer
     4. (read user input)
        if size = 0, display error (Group Size can not be 0!) and return to answer screen
        if size < 3, send to small couples tables
        if size >2, <6, send to small family tables
        if size >5, <11, send to big family / meeting tables
        if size >10, display error (You must reserve multiple tables for group sizes >11)
      store group size if success,
6.   Please Enter the Date you want to Come, up to a month in advance, in the format, yyyy-mm-dd xx : xx (Military Time) to yyyy-mm-dd xx : xx
7.   read user input
8. if time chosen > 3 hours, error, "You can not spend more than 3 hours for one reservation."
   if date chosen > 1 month after , make error appear (Date can not be more than one month in adavance!)
   if date chosen < today, make error appear (Date can not be in the past!)
   store date chosen if success,
9. If all previous steps succeed, say, "Thank You! Press Y if all of the following information is correct and to book your reservation, N if not"
    (Name: Stored Name)
   (Group Size: Stored group size)
   (Date of Reservation)
   scan user input if y is pressed, store all info and turn table(xx)booked to true for date and time (xx)
   if n is pressed, delete all info Output/end: Thank You!


**Step 2**
building the project


**Step 3** 
debugging
issue: people around me had a hard time entering a specific date and time, so i made an example in the code to help.
<img width="1529" height="827" alt="image" src="https://github.com/user-attachments/assets/bd46930d-6328-4718-ad9c-fbee6180b168" />










