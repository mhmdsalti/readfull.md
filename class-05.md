# Reading

## CHAPTER 5 IMAGES

### There are many reasons why you might want to add an image to a web page: you might want to include a logo, photograph, illustration, diagram, or chart

### There are several things to consider when selecting and preparing images for your site, but taking time to get them right will make it look more attractive and professional

## Choosing Images for Your Site

### A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one

## Storing Images on Your Site

### If you are building a site from scratch, it is good practice to create a folder for all of the images the site uses

## Adding Images

### To add an image into the page you need to use an < img > element. This is an empty element (which means there is no closing tag). It must carry the following two attributes

1. (src)This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. (Here you can see that the images are in a child folder called images
2. (alt) This provides a text description of the image which describes the image if you cannot see it.

## Height & Width of Images

### (height) This specifies the height of the image in pixels and (width) This specifies the width of the image in pixels

## Aligning Images Horizontally

1. left This aligns the image to the left (allowing text to flow around its right-hand side)
2. right This aligns the image to the right (allowing text to flow around its left-hand side).
3. top This aligns the first line of the surrounding text with the top of the image.
4. middle This aligns the first line of the surrounding text with the middle of the image
5. bottomThis aligns the first line of the surrounding text with the bottom of the image.

## Figure and Figure Caption

### < figure > Images often come with captions. HTML5 has introduced a new < figure > element to contain images and their caption so that the two are associated. You can have more than one image inside the < figure > element as long as they all share the same caption

### < figcaption > The < figcaption > element has been added to HTML5 in order to allow web page authors to add a caption to an image.Before these elements were created there was no way to associate an < img > element with its caption

## Summary IMAGES

1. The < img > element is used to add images to a web page.
2. You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the content of an image.
3. You should save images at the size you will be using them on the web page and in the appropriate format.
4. Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.

## CHAPTER 11 COLORS

## Color can really bring your pages to life

## forground color : The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways

1. rgb values These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)
2. hex codes These are six-digit codes that represent the amount of red, green and bluein a color, preceded by a pound or hash # sign. For example: #ee3e80
3. color names There are 147 predefined color names that are recognized by browsers. For example: DarkCyan

## We look at these three different ways of specifying colors on the next double-page spread

## CSS3 has also introduced another way to specify colors called HSLA

## Background Color

## CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box , You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names , If you do not specify a background color, then the background is transparent , By default, most browser windows have a white background, but browser users can set a background color for their windows, so if you want to be sure that the background is white you can use the background-color property on the (body) element

## Understanding Color

## Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker

## Computer monitors are made up of thousands of tiny squares called pixels (if you look very closely at your monitor you should be able to see them).When the screen is not turned on, it's black because it's not emitting any light. When it's on, each pixel can be a different color, creating a picture.The color of every pixel on the screen is expressed in terms of a mix of red, green, and blue — just like on a television screen

## RGB ValuesValues for red, green, and blue are expressed as numbers between 0 and 255

## Hex CodesHex values represent values for red, green, and blue in hexadecimal code

## Color NamesColors are represented by predefined names. However, they are very limited in number

## Hue is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue

## SaturationSaturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray

## Brightness (or "value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the color would be very dark

## Contrast : When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible

## Text is harder to read when there is low contrast between background and foreground colors

## Text is easier to read when there is higher contrast between background and foreground colors

## For long spans of text, reducing the contrast a little bit improves readability

## A lack of contrast is particularly a problem for those with visual impairments and color blindness , If you want people to read a lot of text on your page, however, then too much contrast can make it harder to read, too , You can reduce contrast by using dark gray text on a white background or an off-white text on a dark background  , It also affects those with poor monitors and sunlight on their screens (which is increasingly common as people use handheld devices outdoors)

## Summary

1. Color not only brings your site to life but also helps convey the mood and evokes reactions
2. There are three ways to specify colors in CSS: RGB values, hex codes, and color names
3. Color pickers can help you find the color you want.
4. It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).
5. CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
6. CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.

## CHAPTER 12 TEXT

## The properties that allow you to control the appearance of text can be split into two groups

1. Those that directly affect the font and its appearance (including the typeface, whether it is regular, bold or italic, and the size of the text)
2. Those that would have the same effect on text no matter what font you were using (including the color of text and the spacing between words and letters)

## Typeface Terminology

1. Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.
2. Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.
3. Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)
4. Cursive fonts either have joining strokes or other cursive characteristics, such as handwriting styles.
5. Fantasy fonts are usually decorative fonts and are often used for titles. They're not designed for long bodies of text.

## Specifying Typefaces font-family

### The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies

### The value of this property is the name of the typeface you want to use

### The people who are visiting your site need the typeface you have specified installed on their computer in order for it to be displayed

### You can specify a list of fonts separated by commas so that, if the user does not have your first choice of typeface installed, the browser can try to use an alternative font from the list

## Size of Type font-size

### The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are

1. Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is followed by the letters px.
2. percentagesThe default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px

## Type Scales

### You may have noticed that programs such as Word, Photoshop and InDesign offer the same sizes of text

### This is because they are set according to a scale or ratio that was developed by European typographers in the sixteenth century

## Summary TEXT

1. There are properties to control the choice of font, size, weight, style, and spacing.
2. There is a limited choice of fonts that you can assume most people will have installed.
3. If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.
4. You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.
5. You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link
