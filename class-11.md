# Reading

## Chapter 16 Images

## Controlling sizes of images in Css

### You can control the size of an image using the width and height properties in CSS, just like you can for any other box

### Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download

## Aligning images Using Css

### using the < img > element's align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved -

1. The float property is added to the class that was created to represent the size of the image (such as the small class in our
example).
2. New classes are created with names such as align-left or align-right to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image.

## Centering images Using Css

### By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a blocklevel element using the display property with a value of block

### Once it has been made into a block-level element, there are two common ways in which you can horizontally center an image -

1. On the containing element, you can use the text-align property with a value of center
2. On the image itself, you can use the use the margin property and set the values of the left and right margins to auto

## Background Images

### The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box

## Repeating Images

### The background-repeat property can have four values -

1. repeat The background image is repeated both horizontally and vertically (the default way it is shown if the backgroundrepeat property isn't used).
2. repeat-x The image is repeated horizontally only
3. repeat-y The image is repeated vertically only.
4. no-repeat The image is only shown once

## Background Position

### When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed

## Summary IMAGES

1. You can specify the dimensions of images using CSS. This is very helpful when you use the same sized images on several pages of your site.
2. Images can be aligned both horizontally and vertically using CSS.
3. You can use a background image behind the box created by any element on a page.
4. Background images can appear just once or be repeated across the background of the box.
5. You can create image rollover effects by moving the background position of an image.
6. To reduce the number of images your browser has to load, you can create image sprites.

## Chapter 19 Practical Information

## Search Engine Optimization (SEO)

### Search engine optimization (or SEO) is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers

### In every page of your website there are seven key places where keywords (the words people might search on to find your site) can appear in order to improve its findability ->

1. Page Title The page title appears at the top of the browser window or on the tab of a browser. It is specified in the < title > element which lives inside the < head > element.
2. URL / Web Address The name of the file is part of the URL. Where possible, use keywords in the file name.
3. Headings If the keywords are in a heading < hn > element then a search engine will know that this page is all about that subject and give it greater weight than other text
4. Text Where possible, it helps to repeat the keywords in the main body of the text at least 2-3 times. Do not, however, over-use these terms, because the text must be easy for a human to read.
5. Link Text Use keywords in the text that create links between pages(rather than using generic expressions such as "click here").
6. Image Alt Text Search engines rely on you providing accurate descriptions of images in the alt text. This will also help your images show up in the results of image-based searches.
7. Page Descriptions The description also lives inside the < head > element and is specified using a < meta > tag. It should be a sentence that describes the content of the page. (These are not shown in the browser window but they may be displayed in the results pages of search engines.)

## Summary PRACTICAL INFORMATION

1. Search engine optimization helps visitors find your sites when using search engines.
2. Analytics tools such as Google Analytics allow you to see how many people visit your site, how they find it, and what they do when they get there.
3. To put your site on the web, you will need to obtain a domain name and web hosting.
4. FTP programs allow you to transfer files from your local computer to your web server.
5. Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website tools (to save you writing them from scratch)

## Chapter 9 (js book) pages

## SELECTING ELEMENTS BY TAG NAME

### The get El ementsByTagName () method allows you to select elements using their tag name

### The element name is specified as a parameter, so it is placed inside the parentheses and is contained by quote marks

### Note that you do not include the angled brackets that surround the tag name in the HTML (just the letters inside the brackets)

## SELECTING ELEMENTS USING CSS SELECTORS

### querySe 1 ector() returns the first element node that matches the CSS-style selector. querySe 1ectorA11 () returns a Nodelist of all of the matches

### Both methods take a CSS selector as their only parameter. The CSS selector syntax offers more flexibility and accuracy when selecting an element than

### just specifying a class name or a tag name, and should also be familiar to front-end web developers who are used to targeting elements using CSS

## Repeating actions for an entire nodelist

### when you have a nodelist , you can loop though each node in the collection and apply the same statements to each

## LOOPING THROUGH A NODELIST

### If you want to apply the same code to numerous elements, looping through a Nodelist is a powerful technique

### It involves finding out how many items are in the Nodelist, and then setting a counter to loop through them, one-by-one

### Each time the loop runs, the script checks that the counter is less than the total number of items in the Nodelist

