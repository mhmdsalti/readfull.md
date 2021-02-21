# Reading

## Drawing text

### The canvas rendering context provides two methods to render text ->

1. fillText(text, x, y [, maxWidth]) -> Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

2. strokeText(text, x, y [, maxWidth]) -> Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

## Styling text

### we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas

1. font = value --> The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
2. textAlign = value --> Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
3. textBaseline = value --> Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
4. direction = value --> Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

### These properties might be familiar to you, if you have worked with CSS before

## Colors

## If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle

1. fillStyle = color --> Sets the style used when filling shapes.
2. strokeStyle = color --> Sets the style for shapes' outlines.

### color is a string representing a CSS < color >, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000)

## Transparency

### In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style

#### globalAlpha = transparencyValue

### The globalAlpha property can be useful if you want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors

### The rgba() function is similar to the rgb() function but it has one extra parameter. The last parameter sets the transparency value of this particular color. The valid range is again between 0.0 (fully transparent) and 1.0 (fully opaque)

## Shadows

### Using shadows involves just four properties

1. shadowOffsetX = float --> Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
2. shadowOffsetY = float --> Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
3. shadowBlur = float --> Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
4. shadowColor = color --> A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.

## Drawing shapes with canvas

## The grid

### Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default

## Drawing rectangles

### Unlike SVG, < canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes

### First let's look at the rectangle. There are three functions that draw rectangles on the canvas

1. fillRect(x, y, width, height) --> Draws a filled rectangle.
2. strokeRect(x, y, width, height) --> Draws a rectangular outline.
3. clearRect(x, y, width, height) --> Clears the specified rectangular area, making it fully transparent.

## Drawing paths

### Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps

1. First, you create the path.
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it.

#### Here are the functions used to perform these steps

1. beginPath() --> Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
2. Path methods -->Methods to set different paths for objects.
3. closePath() --> Adds a straight line to the path, going to the start of the current sub-path.
4. stroke() --> Draws the shape by stroking its outline.
5. fill()-->Draws a solid shape by filling the path's content area.

#### The first step to create a path is to call the beginPath(). Internally, paths are stored as a list of sub-paths (lines, arcs, etc) which together form a shape. Every time this method is called, the list is reset and we can start drawing new shapes

#### The second step is calling the methods that actually specify the paths to be drawn. We'll see these shortly

#### The third, and an optional step, is to call closePath(). This method tries to close the shape by drawing a straight line from the current point to the start. If the shape has already been closed or there's only one point in the list, this function does nothing

## Basic usage of canvas

### At first sight a < canvas> looks like the < img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the < canvas> element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted

### The id attribute isn't specific to the < canvas> element but is one of the global HTML attributes which can be applied to any HTML element (like class for instance). It is always a good idea to supply an id because this makes it much easier to identify it in a script

### The < canvas> element can be styled just like any normal image (margin, border, background…). These rules, however, don't affect the actual drawing on the canvas. We'll see how this is done in a dedicated chapter of this tutorial. When no styling rules are applied to the canvas it will initially be fully transparent

## Fallback content

### The < canvas> element differs from an < img> tag in that, like for < video>, < audio>, or < picture> elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers

### Providing fallback content is very straightforward: just insert the alternate content inside the < canvas> element. Browsers that don't support < canvas> will ignore the container and render the fallback content inside it. Browsers that do support < canvas> will ignore the content inside the container, and just render the canvas normally

## Required </canvas> tag

### As a consequence of the way fallback is provided, unlike the < img> element, the < canvas> element requires the closing tag (</canvas>). If this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed

### If fallback content is not needed, a simple < canvas id="foo" ...></canvas> is fully compatible with all browsers that support canvas at all

## The rendering context

### The < canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. Other contexts may provide different types of rendering; for example, WebGL uses a 3D context based on OpenGL ES

### The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The  < canvas> element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context. For 2D graphics, such as those covered by this tutorial, you specify "2d" to get a CanvasRenderingContext2D
