# reading

## CHAPTER 2

## When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page

1. Structural markup: the elements that you can use to describe both headings and paragraphs
2. Semantic markup: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on

## HEADINGS

### HTML has six "levels" of headings

1. < h1 >
2. < h2 >
3. < h3 >
4. < h4 >
5. < h5 >
6. < h6 >

## < h1 > is used for main headings

## < h2 > is used for subheadings

## Browsers display the contents of headings at different sizes. The contents of an < h1 > element is the largest, and the contents of an < h6 > element is the smallest

## PARAGRAPHS

### To create a paragraph, surround the words that make up the paragraph with an opening   < p> tag and closing </p> tag

## Bold & Italic

### By enclosing words in the tags < b> and </b> we can make characters appear bold

### By enclosing words in the tags < i> and </i> we can make characters appear italic

## Superscript & Subscript

### The < sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power

### The < sub> element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas

## Line Breaks & Horizontal Rules

### if you wanted to add a line break inside the middle of a paragraph you can use the line break tag < br />

### To create a break between themes — such as a change of topic in a book or a new scene in a play — you can add a horizontal rule between sections using the < hr /> tag

## Strong & Emphasis

### The use of the < strong> element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis.By default, browsers will show the contents of a < strong> element in bold

### The < em> element indicates emphasis that subtly changes the meaning of a sentence.By default browsers will show the contents of an < em> element in italic

## Quotations

### The < blockquote> element is used for longer quotes that take up an entire paragraph. Note how the < p> element is still used inside the < blockquote> element

### Browsers tend to indent the contents of the < blockquote> element, however you should not use this element just to indent a piece of text — rather you should achieve this effect using CSS

### The < q> element is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around the  < q> element, however Internet Explorer does not — therefore many people avoid using the < q> element

## Abbreviations & Acronyms

### If you use an abbreviation or an acronym, then the < abbr > element can be used. A title attribute on the opening tag is used to specify the full term

## Citations &Definitions

### When you are referencing a piece of work such as a book, film or research paper, the   < cite> element can be used to indicate where the citation is from

### In HTML5, < cite> should not really be used for a person's name — but it was allowed in HTML 4, so most people are likely to continue to use it

#### Browsers will render the content of a < cite> element in italics

### The first time you explain some new terminology (perhaps an academic concept or some jargon) in a document, it is known as the defining instance of it .   The  < dfn> element is used to indicate the defining instance of a new term

## Author Details

### The < address> element has quite a specific use: to contain contact details for the author of the page.It can contain a physical address, but it does not have to. For example, it may also contain a phone number or email address

## Changes to Content

### The < ins> element can be used to show content that has been inserted into a document, while the < del> element can show text that has been deleted from it

### The < s> element indicates something that is no longer accurate or relevant (but that should not be deleted).Visually the content of an < s> element will usually be displayed with a line through the center

## SUMMARY for chapter 2

1. HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs)
2. They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation)

## CHAPTER 10

### CSS Associates Style rules with HTML elements

### CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration

### p  { font-family: Arial; }

### p is selector and {this is declaration}

### This rule indicates that all < p > elements should be shown in the Arial typeface

> Selectors indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas
> Declarations indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon

## CSS Properties Affect How ElementsAre Displayed

### CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify several properties in one declaration, each separated by a semi-colon

## Using External CSS

### The < link> element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the < head> element. It should use three attributes

1. href This specifies the path to the CSS file (which is often placed in a folder called css or styles)
2. typeThis attribute specifies the type of document being linked to. The value should be text/css
3. relThis specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file

## Using Internal CSS

### < style> You can also include CSS rules within an HTML page by placing them inside a < style> element, which usually sits inside the < head> element of the page

### The < style> element should use the type attribute to indicate that the styles are specified in CSS. The value should be text/css

## CSS Selectors

### CSS selectors are case sensitive, so they must match element names and attribute values exactly

1. Universal Selector : Applies to all elements in the documen  for example * {}
2. Type Selector : Matches element names for example h1, h2, h3 {}
3. Class Selector : Matches an element whose class attribute has a value that matches the one specified after the period (or full stop) symbol for example .note {} Targets any element whose classattribute has a value of note or p.note {}Targets only < p> elements whose class attribute has a value of note
4. ID Selector : Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol such as #introduction {}
5. Child Selector : Matches an element that is a direct child of anothe such as li>a {}Targets any < a> elements that are children of an < li> element (but not other < a> elements in the page)
6. Descendant Selector : Matches an element that is a descendent of another specified element (not just a direct child of that element) such as p a {}Targets any    < a> elements that sit inside a < p> element, even if there are other elements nested between them
7. Adjacent Sibling Selector : Matches an element that is the next sibling of another such as : h1+p {}Targets the first < p> element after any < h1> element (but not other < p> elements)
8. General Sibling Selector : Matches an element that is a sibling of another, although it does not have to be the directly preceding element such as : h1~p {}If you had two < p> elements that are siblings of an < h1> element, this rule would apply to both

## SUMMARY for chapter 10

1. CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look
2. Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like)
3. Different types of selectors allow you to target your rules at different elements.
4. Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface
5. CSS rules usually appear in a separate document, although they may appear within an HTML page.

## CHapter 2  basic Javascript

## STATEMENTS

>A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.

## COMMENTS

>You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code
>/* This script displays a greeting to the user based upon the current time. It is an example from JavaScript & jQuery book **/

## WHAT Is a VARIABLE

>A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.

## HOW TO DECLARE VARIABLES

### before you can use a variable you need to announce that you want to use it , this invloves creating the variable and givinr it a name

> var name ;
> var is a keyword and name is a variable name

### how to assign  a value for variable

> var name = 3 ;

## DATA TYPES

1. NUMERIC DATA TYPE : numeric data type handles numbers
2. STRING DATA TYPE :the  strings data type consists of letters and other characters.
3. BOOLEAN DATA TYPE : boolean data types can have one of two values: true or false.

## RULES FOR NAMING VARIABLES

1. The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start with a number.
2. The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a dash(-) or a period (.) in a variable name.
3. You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something. For example, var is a keyword used to declare a variable. Reserved words are ones that may be used in a future version of JavaScript
4. score and Score would be different variable names, but it is bad practice to create two variables that have the same name using different cases.
5. use a name that describes the kind of information that the variable stores. For example, fi rstName might be used to store a person's first name, l astNarne for their last name, and age for their age.
6. if your variable name is made of more than one word, use a capital letter for the first letter of every word after the first word. For example, fi rstName rather than fi rstnarne (this is referred to as camel case). You can also use an underscore between each word (you cannot use a dash).

## ARRAYS

### An array is a special type of variable. It doesn't just store one value; it stores a list of values

### You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array)

>such as var colors;  
 colors ['white', 'black', 'custom'] ;

## VALUES IN ARRAYS

### Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one)

## EXPRESSIONS

### An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions

1. EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE
2. EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE

## OPERATORS

### Expressions rely on things called operators; they allow programmers to create a single value from one or more values

1. ASSIGNMENT OPERATORS
2. ARITHMETIC OPERATORS
3. STRING OPERATORS There is just one string operator: the+ symbol. It is used to join the strings on either side of it. such as var firstName = 'Ivy '; var lastName = 'Stone'; var fulName = firstName + lastName =
4. COMPARISON OPERATORS
5. LOGICAL OPERATORS

## ARITHMETIC OPERATORS

1. ADDITION + Adds one value to another
2. SUBTRACTION Subtracts one value from another
3. DIVISION / Divides two values
4. MULTIPLICATION * Multiplies two values using an asterisk
5. INCREMENT + + Adds one to the current number
6. DECREMENT -- Subtracts one from the current number
7. MODULUS % Divides two values and returns the remainder

## SUMMARY for chapter 2 basic Javascript

1. A script is made up of a series of statements. Each statement is like a step in a recipe.
2. Scripts contain very precise instructions. For example, you might specify that a value must be remembered before creating a calculation using that value
3. Variables are used to temporarily store pieces of information used in the script.
4. Arrays are special types of variables that store more than one piece of related information
5. JavaScript distinguishes between numbers (0-9), strings (text), and Boolean values (true or false).
6. Expressions evaluate into a single value.
7. Expressions rely on operators to calculate a value

## Chapter 4 decision and loops

## Decision making

### there are often several places in a script where decisions are mafe that detrmine which lines of code should be run next . flowcharts can help you plan for there occasions

## evaluating conditions and conditional statements

## there are two components to a decision

1. an expression is evaluated which returns a value
2. a conditional statement says what to do in a given situation

## the first thing we have here is about the COMPARISON OPERATORS

1. == is equal to this operator compares two values
2. != is not equal to this operator compares two values to see if they are not the same
3. === strict equal to this operator compares two values to check that both the data type and value are the same
4. !==  strict not equal to this operator compares two values to check that both the data type and value are not the same
5. > greater than this operator check if the number on the left is greater than the number on the right
6. < less than this operator check if the number on the left is less than the number on the right
7. >= greater than or eqaul to this operator check if the number on the left is greater than the number on the right or equal to it
8. <= less than or equal to this operator check if the number on the left is less than the number on the right or equal to it

## the second thing we hvae here is about the LOGICAL OPERATORS , it return single calues of true or false

> && (and) operator this tests more than one condition

- (true && true returns true)
- (true && false returns false)
- (false && true returns false)
- (false && false returns false)

> (or) operator this test at least one condition

- (true || false rutruns true)
- (false || true rutruns true)
- (true || true rutruns true)
- (false || false rutruns false)

> ! (not) operator this take a single boolean value and inverts it

- !true returns false
- !false returns true

## the third and last thing is about if statements

### the if statment evaluates a condition if the condition evaluates to true any statemnts in the subsequent code block are executed

> if ( score >= 50 ){congratulate();}
> if is the keyword (condition){code to execute if value is true}

## if ... else statments

### the if ... else statement checks a condition if it resolves to true the first code block is executed if the condition resolves to false the second code block is run instead

>if (score >= 50 ){congratulate();} else {encourage ();}
