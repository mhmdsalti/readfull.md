# Reading

## chapter 3 LISTS

### HTML provides us with three different types

1. (Ordered lists) are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number.
2. (Unordered lists) are lists that begin with a bullet point (rather than characters that indicate order).
3. (Definition lists) are made up of a set of terms along with the definitions for each of those terms.

## ORDER LIST

### The ordered list is created with the < ol > element

### Each item in the list is placed between an opening < li > tag and a closing < /li > tag. (The listands for list item.)

## UNORDERED LIST

### The unordered list is created with the < ul > element

### Each item in the list is placed between an opening < li > tag and a closing </li> tag. (The listands for list item.)

## DEFINITION LIST

### The definition list is created with the < dl > element and usually consists of a series of terms and their definitions.Inside the < dl > element you will usually see pairs of < dt > and < dd > elements

### < dt > This is used to contain the term being defined (the definition term)

### < dd > This is used to contain the definition

## NESTED LIST

### You can put a second list inside an < li > element to create a sublist or nested list

## SUMMARY

1. There are three types of HTML lists: ordered, unordered, and definition.
2. Ordered lists use numbers.
3. Unordered lists use bullets.
4. Definition lists are used to define terminology.
5. Lists can be nested inside one another.

> NEW CHAPTER

## CHAPTER 13 BOXES

## Box Dimensions (width, height)

### By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties

### The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size

## Limiting Width (min-width, max-width)

### Some page designs expand and shrink to fit the size of the user's screen. In such designs, the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide

## Limiting Height (min-height, max-height)

### In the same way that you might want to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the min-height and max-height properties

## Overflowing Content overflow

### The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values

### hiddenThis property simply hides any extra content that does not fit in the box

### scrollThis property adds a scrollbar to the box so that users can scroll to see the missing content

## Border, Margin & Padding

### Every box has three available properties that can be adjusted to control its appearance

1. BorderEvery box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.
2. MarginMargins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
3. PaddingPadding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents

## White space & Vertical Margin

### The padding and margin properties are very helpful in adding space between various items on the page

### Designers refer to the space between items on a page as white space. Imagine you had a border around a box. You would not want the text to touch this border or it would become harder to read , Or, imagine you had two boxes sitting side by side (each with a black border). You would not necessarily want the boxes to touch edges as this would make the line look twice as thick on the facing sides

## Border Width border-width

### The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of the following values: thin-medium-thick

### (You cannot use percentages with this property.)You can control the individual size of borders using four separate properties:border-top-width border-right-width border-bottom-width border-left-width

## Border Style border-style

1. (solid) a single solid line
2. (dotted) a series of square dots(if your border is 2px wide, then the dots are 2px squared with a 2px gap between each dot)
3. (dashed) a series of short lines
4. (double) two solid lines (the value of the border-width property creates the sum of the two lines)
5. (ridge) appears to stick out from the page
6. (inset) appears embedded into the page
7. (outset) looks like it is coming out of the screen
8. hidden / none no border is shown

## SUMMARY 2

1. CSS treats each HTML element as if it has its own box.
2. You can use CSS to control the dimensions of a box.
3. You can also control the borders, margin and padding for each box with CSS.
4. It is possible to hide elements using the display and visibility properties.
5. Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
6. Legibility can be improved by controlling the width of boxes containing text and the leading.
7. CSS3 has introduced the ability to create image borders and rounded borders.

## Chapter 2: “Basic JavaScript Instructions

## ARRAYS

### An array is a special type of variable. It doesn't just store one value; it stores a list of values

## CREATING AN ARRAY

### You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array). The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array. This technique for creating an array is known as an array literal. It is usually the preferred method for creating an array. You can also write each value on a separate line -> colors= ['white', 'black', 'custom'];)

## VALUES IN ARRAYS

### Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one)

## ACCESSING & CHANGING VALUES IN AN ARRAY

## Chapter 4: “Decisions and Loops”

## SWITCH STATEMENTS

### A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value

### (SWITCH) You have a default option that is run if none of the cases match. ( If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing better performance than multiple if statements)

## TYPE COERCION & WEAK TYPING

### If you use a data type JavaScript did not expect, it tries to make sense of the operation rather than report an error

### JavaScript can convert data types behind the scenes to complete an operation. This is known as type coercion. For example, a string 'l ' could be converted to a number 1 in the following expression:(' 1' > 0). As a result, the above expression would evaluate to true

### JavaScript is said to use weak typing because the data type for a value can change. Some other languages require that you specify what data type each variable will be. They are said to use strong typing

## TRUTHY & FALSY VALUES

### due to type coercion, every value in JavaScript can be treated as if it were true or false; and this has some interesting side effects

### Falsy values are treated as if they are fa 1 se. The table to the left shows a hi ghScore variable with a series of values, all of which are falsy. falsy values can also be treated as the number ()

### truthy values are treated as if they are true. Almost everything that is not in the falsy table can be treated as if it were true . Truthy values can also be treated as the 1

### switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match)
