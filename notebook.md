## Table of Contents
- [Blocks](#blocks)
  
 - [Concepts](#concepts)
   
 - [Vocabulary For Robotics](#vocabulary)
   
- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)

  - [Headings](#headings)

  - [Text Formatting](#text-formatting).

- [Vocab For Advanced Computer Science](#vocab)
  
- [Code Examples](#code-examples)
  
  - [Print Statements](#print-statements)
    
- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)

 

 

## Vocab


<details>
  <summary>algorithm</summary>
    Step-by-step instructions. 
  
    Example: The steps to making cookies and a method we use for long math problems are both examples of algorithms.
</details>

<details>
  <summary>sequencing</summary>
    The order things happen in.

    Example: Brushing your teeth might consist of these steps: Put toothpaste on the toothbrush. Use the toothbrush to clean your teeth.
</details>

  <details>
   <summary>selection</summary>
   The Parts of an algorithm where choices are made.
  
    Example: Making a choice to donate to charity after an algorithm adds up the total cost of your groceries.
</details>

<details>
  <summary>iteration</summary>
    The parts of your algorithm that repeat.
  
    Example: Adding a cost over and over again, repeating the sequence, is iteration.
</details>

<details>
  <summary>java</summary>
    A programming language different than Javascript
</details>

<details>
  <summary>object-oriented-language</summary>
    A versatile programming language because of its modularity, reusability, and easier maintenance due to organized code and encapsulated data.
</details>

<details>
  <summary>procedural-language</summary>
    A language using a linear top-down approach, good for simple projects but hard to maintain for larger projects.
</details>

<details>
  <summary>class</summary>
    A type of blueprint in Java that defines the behavior of objects you create from it.
</details>

<details>
  <summary>method</summary>
    A block of code in a class that does a certain task when called.
</details>

<details>
  <summary>console</summary>
    A place where programs can print to.
</details>

<details>
  <summary>commenting</summary>
    an informative comment in your program, not meant to be run.
</details>

<details>
  <summary>internal-documentation</summary>
    a link that takes a user to a different area in the same site.
</details>

<details>
  <summary>external-documentation</summary>
    information kept out the source files to help others understand your code.
</details>

<details>
  <summary>varuables</summary>
    A variable is something that holds a value
</details>

 <details>
  <summary>strings</summary>
    Characters enveloped in quotation marks
</details>

 <details>
  <summary>integers</summary>
    data type holding a number value
</details>

 <details>
  <summary>double</summary>
    data type h0olding a decimal
</details>

 <details>
  <summary>character</summary>
    a data type holding a single character
</details>

 <details>
  <summary>boolean</summary>
    a data type that holds either a true or false.                                                                                  
</details>


 <details>
  <summary>cameCase</summary>
    a way of writing without spaces, starting with a non-capitalized word, and capitalizing every word after it with no spaces
</details>

## Code Examples
 
  ### Print Statements
  ```java
  public class Hello {
      public static void main(String[] args) {
          System.out.println("Hello World!");
      }
  }
  ```
   **System** accesses a Java class that's built into the language
  
  **out** is short for "output".
  
  **println** is short for "print line".

### Commenting


```java
public class Example {
  public static void main(String[] args) {
    // comment //
  }
}
```
// // or /* */ on either end to start and end comments

## Blocks


Name: Hat Block

Shape/Type: Round on the top with a connector to the bottom to connect with stack blocks

What It Does: Whenever the condition of the hat block is fulfilled, it runs the code.

Example: When Downeye detects object, move forward

<img width="320" height="214" alt="image" src="https://github.com/user-attachments/assets/56e0d781-1a34-4929-8fd3-eb1c68d77d28" />

Name: Stack / Command Block

Shape/Type: Connecter on top and on bottom to attach other of the same block type

What It Does: It runs simple instructions like movement

Example: A stack block that moves the robot 100mm and then turns right

<img width="489" height="227" alt="image" src="https://github.com/user-attachments/assets/5903772a-17d4-4668-b528-5d51fbef9594" />

Name:C-block

Shape/Type: is a c, stack blocks can be placed inside it and above or below it, hexagonal blocks can be placed inside if its a conditional

What It Does: blocks can be placed inside it to run a conditional.

Example: A conditional can fit a hexagonal detect block, both repeats and conditionals attach to stack blocks inside and outside

<img width="493" height="498" alt="image" src="https://github.com/user-attachments/assets/589c6348-d233-4734-87e2-b580a7acec9e" />

Name: Reporter / Oval block

Shape/Type: Oval, no extrusions

What It Does: it can be put inside hexagonal blocks and stack blocks to do equations for values, also can be used for variables

Example: variables can be fit inside hexagonals to find new values for them through equations

<img width="420" height="248" alt="image" src="https://github.com/user-attachments/assets/bda48910-2205-4a18-a578-f3eb089361dd" />

Name: Boolean / Hexagonal Block

Shape/Type: A hexagonal shape with typically longer horizontal sides

What It Does: it can serve as a condition or value for conditional blocks.

Example: a boolean or detect hexagonal block is inside a conditional, if either of them occur, the conditional runs.

<img width="439" height="276" alt="image" src="https://github.com/user-attachments/assets/c8eb6e59-fce1-4c0a-b2a8-828349b38900" />

Name: Repeat / Loop Blocks

Shape/Type: A C-shaped block, attaches to stack blocks and can fit ovals if not forever.

What It Does: It is used to repeat stack lines of code for a certain amount of times

Example: A repeat loop of a robot going around a certain area

<img width="332" height="318" alt="image" src="https://github.com/user-attachments/assets/80c0c99c-0243-4b21-adfb-7556342a64df" />

Name: Wait Until Block

Shape/Type: a stack with a hexagonal outcut inside it

What It Does: it waits until an action that fulfills the hexagonal block occurs, then runs code.

Example: If a robot drives forward and is supposed to turn when it reaches value y (in mm) on the y axis, then a wait until block can help

<img width="580" height="399" alt="image" src="https://github.com/user-attachments/assets/9c8a0653-b10c-4c9a-9f6e-a100ce3a8bf5" />

Name: If-then block

Shape/Type: c-block

What It Does: if a condition is fulfilled, it runs a sequential line of code within itself.

Example: if a robot detects an object, it drives forward.

<img width="565" height="303" alt="image" src="https://github.com/user-attachments/assets/5d23d49f-1071-42ee-8c94-45f0fc621f20" />

Name: Forever Block

Shape/Type: c block with no hexagonal

What It Does: runs a line of code forever

Example: an if then block inside a forever block, will forever check the conditional and fulfill it if it is true.

<img width="440" height="461" alt="image" src="https://github.com/user-attachments/assets/556c62a2-d8d8-468d-bf70-a698754a6e4f" />

## Concepts


Name: Sequence

What It Means: the step-by-step order in which instructions run

In My Own Words: The set of instructions done to accomplish a goal.

Example: getting ready for school, school bell schedules, work schedules, getting home and unpacking

 Name: Parameters

What It Means: parameters act as placeholders within a command or function that allow you to pass in different inputs, directly changing what the command does or how it behaves.

In My Own Words: it's purpose is to be something that allows you to test different inputs to help you understand or debug code.

Example: using a slider to determine the effects of a function in math in relation to an x value

 Name: Loops / Iteration

What It Means: a programming structure that repeats a block of code automatically until a specific condition is met

In My Own Words: It repeats one or multiple sets of code.

Example: A robot that pours ink drives in a swirl until an area is filled with ink

 Name: Sensors

What It Means: virtual tools built into the simulated robot that collect data from the virtual playground environment 

In My Own Words: equipment used to find data about a robot's surroundings to help find out what to do

Example: a location sensor to sense where a robot is, to help it find out what path it needs to take to reach a goal.

 Name: Booleans & Conditions

What It Means: A Boolean in coding is a data type that has only one of two values: true or false. A condition (or conditional statement) uses Booleans to help a program make decisions and choose which block of code to run

In My Own Words: A true or false statement that helps a program reach its goal by allowing it to adapt 

Example: If robot doesn't move for 200 seconds, it turns a boolean true, which a conditional uses to try and get the robot free

 Name: Sense -> Think -> Act

What It Means: a foundational three-step programming and computer science framework that describes how a robot interacts with its environment.

In My Own Words: A robot senses its environment, assesses it, and uses an algorithm to help it achieve its goal.

Example: A robot senses its location and whats around it, it thinks about a path to reach its goal, it moves on the path.

 Name: Comparisons

What It Means: evaluating two values to see how they relate to each other

In My Own Words: Comparing two values to find out what to do.

Example: If the risk of something is higher than the reward, don't do it, but if the reward is higher than the risk, do it.

 Name: Coordinates 

What It Means: sets of numbers that give the exact address or position of a point on a graph, a map, or in space

In My Own Words: A pair of x and y values that determine a robot's location

Example: you can be found on any world map using x and y values.

 Name: Conditionals

What It Means: an instruction that tells a program to make a decision and run different blocks of code depending on whether a specific condition is true or false

In My Own Words: if something is true and fulfils a conditional, it runs a sequence.

Example: If you knock over a vase, it will break.

 Name: Patterns

What It Means: reusable, proven blueprints or templates used to solve common, recurring problems in software design

In My Own Words: A re-occuring set of instructions or code that solves a problem

Example: Seeing the same code being used over and over again to solve the problem of a robot hitting a wall on accident and changing course.
 
## Vocabulary


VR Robot + Playground	VR Robot - The Robot used on the website VR Vex dot com. 

Programming Language + Project - The language used to program a set of code.

Behavior + Command - A sequence of code that you give to a robot to perform that sequence.

Drivetrain - components that transfer power from the brain and battery to wheels and other functions.

Loop + Iteration - Repetition of a sequence of code.

Sensor + Bumper Sensor - A sensor used to gather data on the environment around the robot by detecting what bumps into it.

Boolean + Condition + TRUE/FALSE - A Boolean is a statement that holds either a true or false value.

Distance Sensor + Threshold	Distance Sensor - A sensor that gathers data about its environment by calculating the distance between itself and something in front of it.

Coordinate Plane + X/Y Coordinates - A plane with specific values that help determine a location on the plane.

Location Sensor - A sensor that gathers data about its environment by checking its location.

Comment	- A piece of text that is only visible to a coder to provide information on a piece of code like why or how it works

Eye Sensor - a sensor that gathers data about its environment by recognizing the color of whatever it is pointed at.

Conditional Statement	- a statement that runs if and only if a certain value fuffils the conditional.


## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  

This ensures your notes are easy for you (and others) to read later.

## Headings

**When to use:** Organize your notebook into sections (like days, topics, or projects).  

- `#` for the notebook title (use once at the top).  

- `##` for each day or major topic.  

- `###` for subsections (like "Notes", "Practice", "Reflections").  

# Example:

# My Coding Notebook

## Day 1

### Notes

### Practice

# Text Formatting

When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

# Example:

**Class** = a blueprint for objects  

*Remember:* always test your code  

Use `System.out.println()` to print

 

# Code Blocks

When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

# Example:

```java

public class Hello {

    public static void main(String[] args) {

        System.out.println("Hello World!");

    }

}

```

# Lists

When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

# Example:

Define the class
Write the main method
Test your program
Variables

- Loops

- Conditionals

 

# Checklists

When to use: Track progress on assignments or tasks.

# Example:

[x] Complete coding warm-up

- [ ] Finish project draft

- [ ] Reflect on learning

 

# Blockquotes

When to use: Call out notes, reminders, or teacher comments.

# Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

# Tables

When to use: Compare values, track progress, or organize data neatly.

# Example:

| Task        | Status   | Notes          |

|--------------|------------|-----------------| 

| Homework 1  | Done #  | Submitted      |

| Homework 2  | Pending  | Needs review   |

 

# Links & Images

When to use: Add references, resources, or visuals.

# Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  

![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

To make an image that is a link, paste the image, then add the following before it, replacing website address with the link:

<a href="website address">

And after the image info, add: </a>

# Collapsible Sections

When to use: Hide solutions, extended notes, or extra details.

# Example:

<details>

  <summary>Click to reveal solution</summary>

  

System.out.println("Answer: 42");

</details>

 

# Footnotes

When to use: Add references or side notes without cluttering the page.

# Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

# Style Rules

Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

# Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.
