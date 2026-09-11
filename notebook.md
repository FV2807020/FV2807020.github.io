## Table of Contents

- [Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)

  - [Headings](#headings)

  - [Text Formatting](#text-formatting).

- [Vocab](#vocab)
  
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

## Code Examples
 
  ### Print Statements
  ```java
  public class Hello {
      public static void main(String[] args) {
          System.out.println("Hello World!");
      }
  }
  ```
  ---

### Commenting
```java
public class Example {
  public static void main(String[] args) {
    // comment //
  }
}
```
  **System** accesses a Java class that's built into the language
  
  **out** is short for "output".
  
  **println** is short for "print line".

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
