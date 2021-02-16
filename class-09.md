# Reading

## Chapter 7: “Forms"

## Why Forms?

### The best known form on the web is probablythe search box that sits right in the middle of Google's homepage

## Form Controls

### There are several types of form controls that you can use to collect information from visitors to your site

#### ADDING TEXT -

1. Text input (single-line) Used for a single line of text such as email addresses and names

2. Password input Like a single line text box but it masks the characters entered.

3. Text area (multi-line) For longer areas of text, such as messages and comments.

#### Making Choices -

1. Radio buttons For use when a user must select one of a number of options.

2. Checkboxes When a user can select and unselect one or more options.

3. Drop-down boxes When a user must pick one of a number of options from a list

#### Submitting Forms

1. Submit buttons To submit data from your form to another web page

2. Image buttons Similar to submit buttons but they allow you to use an image.

#### Uploading Files -

1. File upload Allows users to upload files (e.g. images) to a website

## How Forms Work

1. A user fills in a form and then presses a button to submit the information to the server.

2. The name of each form control is sent to the server along with the value the user enters or selects.

3. The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.

4. The server creates a new page to send back to the browser based on the information received.

### A form may have several form controls, each gathering different information. The server needs to know which piece of inputted data corresponds with which form element

## Summary FORMS

1. Whenever you want to collect information from visitors you will need a form which lives inside a < form > element.
2. Information from a form is sent in name/value pairs.
3. Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.
4. HTML5 introduces new form elements which make it
easier for visitors to fill in forms.

## Chapter 14: "Lists"

## list-style-type

### The list-style-type property allows you to control the shape or style of a bullet point (also known as a marker). It can be used on rules that apply to the < < ol>, < ul>, and < li> elements

1. Unordered Lists For an unordered list you can use the following values: none, disc , circle ,square
2. Ordered Lists For an ordered (numbered) list you can use the following values: decimal -> 1 2 3 ,decimal-leading-zero -> 01 02 03, lower-alpha -> a b c, upper-alpha -> A B C, lower-roman -> i. ii. iii. , upper-roman -> I II III.

## Summary LISTS, TABLES AND FORMS

1. In addition to the CSS properties covered there are several others that are specifically used to control the appearance of lists, tables, and forms.
2. List markers can be given different appearances using the list-style-type and list-style image properties.
3. Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.
4. Forms are easier to use if the form controls are vertically aligned using CSS.
5. Forms benefit from styles that make them feel more
interactive.

## CHAPTER Chapter 6: "Events"

### When you browse the web, your browser registers different types of events. It's the browser's way of saying, "Hey, this just happened." Your script can then respond to these events

## HOW EVENTS TRIGGER JAVASCRIPT CODE

### When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as event handling

1. Select t he element node(s) you want the script to respond to.
2. Indicate which event on the selected node(s) will trigger the response. Programmers call this binding an event to a DOM node.
3. State the code you want to run when the event occurs. When the event occurs, on a specified element, it will trigger a function. This may be a named or an anonymous function.

### Here you can see how event handling can be used to provide feedback to users filling in a registration form. It will show an error message if their username is too short

1. SELECT ELEMENT the element that users are interacting with is the text input where they enter the username.
2. Specify Event When users move out of the text input, it loses focus, and the blur event fires on this element.
3. CALL CODE When the blur event fires on the username input, it will trigger a function called check kUsername ().This function checks if the username is less than 5 characters.

## EVENT LISTENERS

### Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers

## Event Flow

### HTML elements nest inside other elements . if you hover or click on a link , you will also be hovering or clicking on its parent elements

## Why Flow Matters

### the flow of events only really matters when your code has event handlers on an element and one of its ancestor or descendant elements

## Where Events Occur

### the event object can tell you where the cursor was postioned when an event was triggered

## SUMMARY EVENTS

1. Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
2. Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.
3. When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
4. You can use event delegation to monitor for events that happen on all of the children of an element.
5. The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.
