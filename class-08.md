# Reading

## CHAPTER 15 LAYOUT

## Key Concepts in Positioning Elements

### Building BlocksCSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box

### Block-level elements start on a new lineExamples include:< h1> < p> < ul> < li>

### Inline elements flow in between surrounding textExamples include:< img> < b> < i>

### Containing Elements If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element

## Controlling the Position of Elements

### CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property

### Normal flow Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior (unless you tell the browser to do something else)

### Relative PositioningThis moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow

### Absolute positioning This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page

### To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed. (You will meet these when we introduce the positioning schemes on the following pages.)

### Fixed Positioning This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down the page

### Floating ElementsFloating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow

## Screen Sizes

### Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens

### When designing for print, you always know the size of the piece of paper that your design will be printed on. However, when it comes to designing for the web, you are faced with the unique challenge that different users will have different sized screens

### Since computers have been sold to the public, the size of screens has been steadily increasing. This means that some people viewing your site might have 13 inch monitors while others may have 27+ inch monitors

### The size of a user's screen affects how big they can open their windows and how much of the page they will see. There are also an increasing number of handheld devices (mobile phones and tablets) that have smaller screens

## Screen Resolution

### Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens

## Page Sizes

### Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens)

## Fixed Width Layouts

### Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels

## Liquid Layouts

### Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages

## SUMMARY FOR CHAPTER LAYOUT

1. < div> elements are often used as containing elements to group together sections of a page
2. Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning
3. The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)
4. Pages can be fixed width or liquid (stretchy) layouts.
5. Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
6. Grids help create professional and flexible designs.
7. CSS Frameworks provide rules for common tasks.XYou can include multiple CSS files in one page
