# reading

## All websites use HTML and CSS, but content management systems, blogging software, and e-commerce platforms often add a few more technologies into the mix

## How the Web Works --> When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server

## HTML Uses Elementsto Describe the Structure of Pages

## < html >

> < body >
> < h1 >This is the Main Heading</h1>  
> < p > This text might be an introduction to the rest of  the page. And if the page is a long one it might  be split up into several sub-headings. < p >
> < h2 >This is a Sub-Heading</h2>
> < p> Many long articles have sub-headings so to help  you follow the structure of what is being written.  There may even be sub-sub-headings (or lower-level  headings).</p>  
> < h2 > Another Sub-Heading</h2>
> < p >Here you can see another sub-heading.</p>
> </body>
> </html>

## Tags act like containers. They tell you something about the information that lies between their opening and closing tags

## The opening < html > tag indicates that anything between it and a closing </html> tag is HTML code

## The < body > tag indicates that anything between it and the closing </body> tag should be shown inside the main browser window

## Words between < h1> and </h1> are a main heading

## A paragraph of text appears between these < p > and </p> tags

## Words between < h2 > and </h2> form a sub-heading

## The closing </body> tag indicates the end of what should appear in the main browser window

## The closing </html> tag indicates that it is the end of the HTML code

## HTML pages are text documents

## HTML uses tags (characters that sit inside angled brackets) to give the information they surround special meaning

## Tags are often referred to as elements

## Tags usually come in pairs. The opening tag denotes the start of a piece of content; the closing tag denotes the end

## Opening tags can carry attributes, which tell us more about the content of that element

## Attributes require a name and a value

## To learn HTML you need to know what tags are available for you to use, what they do, and where they can go

## DOCTYPES

### Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included)

## Comments in HTML

### If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:            <!-- comment goes here -->

### It is a good idea to add comments to your code because, no matter how familiar you are with the page at the time of writing it, when you come back to it later (or if someone else needs to look at the code), comments will make it much easier to understand

### Although comments are not visible to users in the main browser window, they can be viewed by anyone who looks at the source code behind the page

## ID Attribute

### Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character).It is important that no two elements on the same page have the same value for their idattributes (otherwise the value is no longer unique)

### for example < p id="pullquote">Every time I view the sea I feel  a calming sense of security, as if visiting my  ancestral home; I embark on a voyage of seeing.</p >

## Class Attribute

### Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page. For example, you might have some paragraphs of text that contain information that is more important than others and want to distinguish these elements, or you might want to differentiate between links that point to other pages on your own site and links that point to external sites

### for example < p class="important">For a one-year period from  November 2010, the Marugame Genichiro-Inokuma  Museum of Contemporary Art (MIMOCA) will host a  cycle of four Hiroshi Sugimoto exhibitions.</p >

## Block Elements

### Some elements will always appear to start on a new line in the browser window. These are known as block level elements

### Examples of block elements are < ul > < li >Science: 21 Nov - 20 Feb 2010/11 < /li > < li >Architecture: 6 Mar - 15 May 2011 < /li > < li > History: 29 May - 21 Aug 2011 < /li > < li >Religion: 28 Aug - 6 Nov 2011 < /li > < /ul > ( ul) means unorder list

## Inline Elements

### Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements

### Examples of inline elements are  Timed to a single revolution of the planet around the sun at a 23.4 degrees tilt that plays out the rhythm of the seasons, this  < em > Origins of Art</em>cycle is organized around four themes: < b > science, architecture, history < /b > and < b > religion < /b >

## GroupingText & Elements In a Block

### For example, you might create a < div> element to contain all of the elements for the header of your site (the logo and the navigation), or you might create a < div> element to contain comments from visitors

### < div > --->  The < div > element allows you to group a set of elements together in one block-level box

### for example < div id="header">< img src="images/logo.gif" alt="Anish Kapoor" />< ul> < li> < a href="index.html">Home</a></li> < li>< a href="biography.html">Biography</a></li> < li>< a href="works.html">Works</a></li> < li>< a href="contact.html">Contact</a></li></ul>                     </div><!-- end of header -->

## The < span> element acts like an inline equivalent of the < div>element. It is used to either

## IFrames

### An iframe is like a little window that has been cut into your page — and in that window you can see another page. The term iframe is an abbreviation of inline frame

### example < iframe width="450" height="350" src="http://maps.google.co.uk/maps?q=moma+new+york&amp;output=embed"> </iframe>

## Information About Your Pages

### The < meta > element lives inside the < head> element and contains information about that web page

### It is not visible to users but fulfills a number of purposes such as telling search engines about your page, who created it, and whether or not it is time sensitive. (If the page is time sensitive, it can be set to expire. )

## Escape Characters

### There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.)

1. < Less-than sign &lt; &#60;
2. > Greater-than sign &gt; &amp;
3. & Ampersand &amp; &#38;
4. " Quotation mark&quot; &#34;
5. ¢ Cent sign &cent; &#162;
6. £ Pound sign &pound; &#163;
7. ¥ Yen sign &yen; &#165;
8. Euro sign &euro; &#8364;
9. © Copyright symbol &copy; &#169;
10. ® Registered trademark &reg; &#174;
11. ™ Trademark &trade; &#8482;
12. ‘ Left single quote &lsquo; &#8216;
13. ' Right single quote &rsquo; &#8217;
14. “ Left double quotes &ldquo; &#8220;
15. ” Right double quotes &rdquo; &#8221;
16. × Multiplication sign &times; &#215;
17. ÷ Division sign&divide; &#247;

## SUMMARY

### DOCTYPES tell browsers which version of HTML you are using

### You can add comments to your code between the <!-- and --> markers

### The id and class attributes allow you to identify particular elements

### The < div> and < span> elements allow you to group block-level and inline elements together

### < iframes> cut windows into your web pages through which other pages can be displayed

### The < meta> tag allows you to supply all kinds of information about your web page

### Escape characters are used to include special characters in your pages such as <, >, and ©

## Headers & Footers

### The < header > and < footer > elements can be used for

1. The main header or footer that appears at the top or bottom of every page on the site
2. A header or footer for an individual < article > or < section > within the page.

## Navigation < nav>

### The < nav> element is used to contain the major navigational blocks on the site such as the primary site navigation

## Articles < article >

### The < article > element acts as a container for any section of a page that could stand alone and potentially be syndicated

## Asides < aside >

### The < aside> element has two purposes, depending on whether it is inside an < article > element or not

1. When the < aside> element is used inside an < article>element, it should contain information that is related to the article but not essential to its overall meaning. For example, a pullquote or glossary might be considered as an aside to the article it relates to
2. When the < aside> element is used outside of an < article>element, it acts as a container for content that is related to the entire page. For example, it might contain links to other sections of the site, a list of recent posts, a search box, or recent tweets by the author

## Sections < section>

### The < section> element groups related content together, and typically each section would have its own heading

## Heading Groups < hgroup>

### The purpose of the < hgroup > element is to group together a set of one or more  < h1 > through < h6 > elements so that they are treated as one single heading

## Figures < figure > < figcaption >

1. It is important to note that the article should still make sense if the content of the < figure > element were moved (to another part of the page, or even to a different page altogether).
2. For this reason, it should only be used when the content simply references the element (and not for something that is absolutely integral to the flow of a page).

### Examples of usage include

1. Images
2. Videos
3. Graphs
4. Diagrams
5. Code samples
6. Text that supports the main body of an article

### The < figure> element should also contain a < figcaption> element which provides a text decription for the content of the  < figure> element. In this example, you can see a < figure> has been added inside the < article> element

## summary

1. The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure
2. The new elements provide clearer code (compared with using multiple < div> elements).
3. Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements
4. To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google

## process and desing

### Every website should be designed for the target audience—not just for yourself or the site owner. It is therefore very important to understand who your target audience is

### It's important to understand who your target audience is, why they would come to your site, what information they want to find and when they are likely to return

## The aim is to create a diagram of the pages that will be used to structure the site. This is known as a  ( site map ) and it will show how those pages can be grouped

### Now that you know what needs to appear on your site, you can start to organize the information into sections or pages

### Site maps allow you to plan the structure of a site

## A wireframe is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require

### Wireframes allow you to organize the information that will need to go on each page

### Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them

### You can differentiate between pieces of information using size, color, and style

### You can use grouping and similarity to help simplify the information you present

## how JavaScript can be used in browsers to make websites more interactive, interesting, and user-friendly

### Learning to program with JavaScript involves

1. Understanding some basic programming concepts and the terms that JavaScript programmers use to describe them
2. Learning the language itself, and, like all languages, you need to know its vocabulary and how to structure your sentences
3. Becoming familiar with how it is applied by looking at examples of how JavaScript is commonly used in websites today

## javaScript allows you to make web pages more interactive by accessing and modifying the content and markup used in a web page while it is being viewd in the browser

## a script is a series of instructions that a computer can follow to achieve a goal

## a browser may use different parts of the script depending on how the user interacts with the web page

## scripts can run different sections of the code in response to the situation around them

## To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it

## Start with  what you want to achieve, and break that down into smaller steps

1. define the goal -- > First, you need to define the task you want to achieve. You can think of this as a puzzle for the computer to solve
2. design the script -- > To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle. This can be represented using a flowchart
3. CODE EACH STEP -- > each of the steps needs to be written in a programming language that the computer understands. In our case, this is JavaScript.

## desiging a script -- > once you know the goal of your script you can work out the individual tasks needed to achieve it . this high-level view of the tasks can be represented using a flowchart

## summary of the ABC of programming

### what is a script and how do i create one

1. script is a series of instructions that a computer can follow to achieve a goal
2. Each time the script runs, it might only use a subset of all the instructions
3. Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task prggrammatically
4. To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help)
5. It is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the . j s extension.
6. The HTML < script > element is used in HTML pages to tell the browser to load the JavaScript file (rather like the < link > element can be used to load a CSS file)
7. If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web page that the browser has created
