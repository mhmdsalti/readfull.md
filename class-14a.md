# Reading

## lesson 7

## Transforms

### With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property

### The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values

### Transform Syntax : The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses

### 2D Transforms : Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth

### Combining Transforms : It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas

### Using multiple transform declarations will not work, as each declaration will overwrite the one above it. The behavior in that case would be the same as if you were to set the height of an element numerous times

### Transform Origin : As previously mentioned, the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used

### The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis

### Individually the values are treated like that of a background image position, using either a length or keyword value. That said, 0 0 is the same value as top left, and 100% 100% is the same value as bottom right. More specific values can also be set, for example 20px 50px would set the origin to 20 pixels across and 50 pixels down the element

### Perspective : In order for three-dimensional transforms to work the elements need a perspective from which to transform. The perspective for each element can be thought of as a vanishing point, similar to that which can be seen in three-dimensional drawings

### 3D Transforms : Working with two-dimensional transforms we are able to alter elements on the horizontal and vertical axes, however there is another axis along which we can transform elements. Using three-dimensional transforms we can change elements on the z axis, giving us control of depth as well as length and width

### Transform Style : On occasion three-dimensional transforms will be applied on an element that is nested within a parent element which is also being transformed. In this event, the nested, transformed elements will not appear in their own three-dimensional space. To allow nested elements to transform in their own three-dimensional plane use the transform-style property with the preserve-3d value

### The transform-style property needs to be placed on the parent element, above any nested transforms. The preserve-3d value allows the transformed children elements to appear in their own three-dimensional plane while the flat value forces the transformed children elements to lie flat on the two-dimensional plane

## lesson 8

## Transitions & Animations

### Transitions : for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes

### There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular

### Animations : Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off

### Customizing Animations : Animations also provide the ability to further customize an element’s behavior, including the ability to declare the number of times an animation runs, as well as the direction in which an animation completes

## Here are 8 really simple effects that will add life to your UI and smiles to your users’ faces

1. fade in : Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.

2. Change color : Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them.

3. Grow & Shrink : To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

4. Rotate elements : CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element

5. Square to circle : A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

6. 3D shadow : 3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces. This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.

7. Swing : Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.

8. Inset border : One of the hottest button styles right now is the ghost button; a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.
