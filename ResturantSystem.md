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
```java
import java.util.Scanner;
import java.time.LocalDateTime;
import java.time.format.DateTimeFormatter;
import java.time.format.DateTimeParseException;
import java.time.Duration;

public class ReservationSystem {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        DateTimeFormatter formatter = DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm");

        System.out.println("Welcome to INSERT RESTAURANT NAME! Here, you will be able to reserve your seat");

        while (true) {
            // 1. Name Input
            System.out.print("Please Enter Your First and Last Name: ");
            String name = scanner.nextLine().trim();
            if (name.isEmpty()) {
                System.out.println("Name cannot be empty. Please try again.\n");
                continue;
            }

            // 2. Group Size Input
            int groupSize = 0;
            String tableType = "";
            boolean validGroup = false;

            while (!validGroup) {
                System.out.print("Please Enter your Group Size In a Single Integer: ");
                try {
                    groupSize = Integer.parseInt(scanner.nextLine().trim());
                    
                    if (groupSize == 0) {
                        System.out.println("Group Size can not be 0!");
                    } else if (groupSize > 10) {
                        System.out.println("You must reserve multiple tables for group sizes >10");
                    } else {
                        // Determine table type based on criteria
                        if (groupSize < 3) {
                            tableType = "small couples tables";
                        } else if (groupSize < 6) {
                            tableType = "small family tables";
                        } else {
                            tableType = "big family / meeting tables";
                        }
                        validGroup = true;
                    }
                } catch (NumberFormatException e) {
                    System.out.println("Invalid input. Please enter a valid integer.");
                }
            }

            // 3. date time setup and scan
            LocalDateTime startDateTime = null;
            LocalDateTime endDateTime = null;
            boolean validDate = false;

            while (!validDate) {
                System.out.println("Please Enter the Date you want to Come (up to a month in advance).");
                System.out.print("Format Example 2026-11-15 18:30 to 2026-11-15 20:30.");
                String dateInput = scanner.nextLine().trim();

                String[] parts = dateInput.split(" to ");
                if (parts.length != 2) {
                    System.out.println("Invalid format. Make sure to use ' to ' between the start and end times.");
                    continue;
                }

                try {
                    startDateTime = LocalDateTime.parse(parts[0].trim(), formatter);
                    endDateTime = LocalDateTime.parse(parts[1].trim(), formatter);
                    LocalDateTime now = LocalDateTime.now();

                    // pretense protection
                    if (startDateTime.isBefore(now)) {
                        System.out.println("Date can not be in the past!\n");
                    } else if (startDateTime.isAfter(now.plusMonths(1))) {
                        System.out.println("Date can not be more than one month in adavance!\n");
                    } else if (Duration.between(startDateTime, endDateTime).toMinutes() > 180) {
                        System.out.println("You can not spend more than 3 hours for one reservation.");
                    } else if (endDateTime.isBefore(startDateTime)) {
                        System.out.println("End time cannot be before start time.\n");
                    } else {
                        validDate = true;
                    }
                } catch (DateTimeParseException e) {
                    System.out.println("Could not parse dates. Ensure you match the pattern exactly (e.g., 2026-11-15 18:30 to 2026-11-15 20:30).\n");
                }
            }

            // 4. confirm
            System.out.println("\n-------------------------------------------");
            System.out.println("Name: " + name);
            System.out.println("Group Size: " + groupSize + " (" + tableType + ")");
            System.out.println("Date of Reservation: " + startDateTime.format(formatter) + " to " + endDateTime.format(formatter));
            System.out.println("-------------------------------------------");
            System.out.print("Thank You! Press Y if all of the following information is correct and to book your reservation, N if not: ");
            
            String confirmation = scanner.nextLine().trim().toUpperCase();

            if (confirmation.equals("Y")) {
                // end / output
                boolean tableBooked = true; 
                System.out.println("\nThank You! Your reservation is confirmed.");
                break; 
            } else {
                // Delete and restart loop
                name = "";
                groupSize = 0;
                startDateTime = null;
                endDateTime = null;
                System.out.println("\nReservation canceled. Restarting form...\n");
            }
        }
        
        scanner.close();
    }
}


```

**Step 3** 
debugging
issue: people around me had a hard time entering a specific date and time, so i made an example in the code to help.
<img width="1529" height="827" alt="image" src="https://github.com/user-attachments/assets/bd46930d-6328-4718-ad9c-fbee6180b168" />










