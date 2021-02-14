# Reading

## Domain Modeling

### Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model. A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams

## Model epic fails videos

## Imagine you've been tasked to build a program that models the popularity of epic fail videos. After months of painstaking research, you've determined that the two essential metrics for gauging popularity are an epic rating and whether or not the video has animals. Since you'll be modeling the popularity of many types of videos—parkour epic fails, corgi epic fails, etc.—you'll want to build self-contained objects with the same attributes and behaviors. That way, when you need to change the algorithm for determining popularity, the changes will be small and targeted

## chapter 6 "tables"

## What's a Table?

### A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results

## Basic Table Structure

1. The < table > element is used to create a table. The contents of the table are written out row by row.
2. You indicate the start of each row using the opening < tr > tag. (The tr stands for table row.) It is followed by one or more < td > elements (one for each cell in that row). At the end of the row you use a closing </tr> tag
3. < td >Each cell of a table is represented using a < td >element. (The td stands for table data.)At the end of each cell you use a closing </td> tag

## Table Headings

### The < th > element is used just like the < td > element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.) Even if a cell has no content, you should still use a < td > or < th > element to represent the presence of an empty cell otherwise the table will not render correctly. (The first cell in the first row of this example shows an empty cell.)Using  < th > elements for headings helps people who use screen readers, improves the ability for search engines to index your pages, and also enables you to control the appearance of tables better when you start to use CSS.You can use the scope attribute on the < th > element to indicate whether it is a heading for a column or a row. It can take the values: row to indicate a heading for a row or col to indicate a heading for a column

## Long Tables

### There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content). These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table (as you will see when you learn about CSS)

1. The headings of the table should sit inside the < thead > element.
2. The body should sit inside the < tbody > element
3. The footer belongs inside the < tfoot > element.

## Summary for chapter 6

1. The < table > element is used to add tables to a web page.
2. A table is drawn out row by row. Each row is created with the < tr > element.
3. Inside each row there are a number of cells represented by the < td > element (or < th > if it is a header).XYou can make cells of a table span more than one row or column using the rowspan and colspan attributes.
4. For long tables you can split the table into a < thead >, < tbody >, and < tfoot >.

## chapter 3 Functions, Methods, and Objects

### the new keyword and the object constructor create a blank object. you can then add properties and methods to the object

### firs you create new object using a combination of the new keyword and the object() constructor function . ( this function is part of the js language and is used to create objects)

### next having created the blank object you can add properties and methods to it using dot notation . each statement that adds a property or method should end with a semicolon

> example vat hotel = new object();

## updating an object

### to update the value of properties use dot notation or square brackets. they work on objects created using literal or constructor notation. to delete a property use the delete keyword

## creating many objects constructor notation

### sometimes you will want several objects to represent similar things . object constructors can use a function as a template for creating objects . first create the template with object properties and methods

## THIS (IT IS A KEYWORD)

### The keyword this is commonly used inside functions and objects. Where the function is declared alters what this means. It always refers to one object, usually the object in which the function operates

## RECAP: STORING DATA

### In JavaScript, data is represented using name/value pairs. To organize your data, you can use an array or object to group a set of related values. In arrays and objects the name is also known as a key

## arrays are objects

### arrays are actually a special type of object . they hold a related set of key/value pairs (like all objects) , but the key for each value is its index number

## array of objects & objects in arrays

### you can combine arrays and objects to create complex data structures : array can store a series of objects ( and remember their order ) . objects can also hold arrays ( as values of their properties)

## three groups of built-in objects

1. browser object model
2. document object model
3. global javascript objects

## creating an instance of the date object

### in order to work with dates you create an instance of the date object. you can then specify the time and date that you want it to represent

## summary of chapter 3

1. Functions allow you to group a set of related statements together that represent a single task.
2. Functions can take parameters (informationJ required to do their job) and may return a value.
3. An object is a series of variables and functions that represent something from the world around you.
4. In an object, variables are known as properties of the object; functions are known as methods of the object.
5. Web browsers implement objects that represent both the browser window and the document loaded into the browser window.
6. JavaScript also has several built-in objects such as String, Number, Math, and Date.Their properties and methods offer functionality that help you write scripts.
7. Arrays and objects can be used to create complex data sets (and both can contain the other).
