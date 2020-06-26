# Responsive Web Design

![resp](https://hackernoon.com/drafts/1tjg32bo.png)

Have you ever wondered how can websites possibly keep up with the millions of screens out there? With responsive website design, your website (and its pages) can adapt and deliver the best experience to users, whether they’re on their desktop, laptop, tablet, or smartphone. For that to happen, though, your website needs a responsive design.

### How does responsive web design work?

Responsive web design works through Cascading Style Sheets (CSS), using various settings to serve different style properties depending on the screen size, orientation, resolution, color capability, and other characteristics of the user’s device. A few examples of CSS properties related to responsive web design include the viewport and media queries.

### Responsive vs. Adaptive vs. Mobile

  * Responsive generally means to react quickly and positively to any change

  * Adaptive means to be easily modified for a new purpose or situation, such as change

  * Mobile means to build a separate website commonly on a new domain solely for mobile users.

### Responsive web design is broken down into three main components, including:

#### Flexible Layouts:

flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.

Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. Reason being, the viewport height and width continually change from device to device. Website layouts need to adapt to this change and fixed values have too many constraints

The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.

   * target ÷ context = result

#### Media Queries

Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation.

It uses the @media rule to include a block of CSS properties only if a certain condition is true. for example:

    @media only screen and (max-width: 600px) {
     body {
          background-color: lightblue;
          }
    }

In this example, If the browser window is 600px or smaller, the background color will be lightblue.

#### Flexible Media

Media that move and scale with our flexible grid is another key feature of a responsive web design. Flexible Media often give web designers a bit of a headache. Loading in huge, oversized images that we scale down using width and height HTML attributes when we want more space for text content on smaller browsing devices is not a good practice for faster web page load times.

Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.
One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.

    img, video, canvas {
        max-width: 100%;
    }


# Float

![float](/img/float.PNG)

CSS *float* Property controls the way an element moves gently in a container or block & another element(like texts) wraps around this element. This also decides which element floats and which doesn’t float.

Float is often used to set up the layout template for a website. In the example below, the sidebar section floats to the left, and the main content section floats to the right. Setting up the different sections using float (as opposed to other techniques such as using a table) makes it easy for the website to behave in a responsive manner. In other words, it can render fine regardless of the screen size of the device used to access the site.

![float website](https://www.1keydata.com/css-tutorial/website-layout-using-float.jpg)

#### The float property has the following possible values:

  * none: no float effect. This is the default.
  * left: floats to the left.
  * right: floats to the right.
  * inherit: inherits the float setting from the parent element.
  * initial: sets the float setting to the default value.

#### Clearing the Float

Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float.

# Don't Overthink It Grids

  * Vast majority of websites use a grid system of some sort
  
  * Simple grid: "Main content area" floated to the left and a "sidebar" floated to the right
  * Basic grid:

       * Main content area column that's 2/3 the width
       * Sidebar column that's 1/3 the width
       * Clear parent element and give it "" content
       * Add gutters
       * Break down content into modules if possible

# CSS Floats Explained By Riding An Escalator

Float elements create two lines, such as an escalator. It allows for content to flow on both the rigth and left of the containing element, making design much more fluid.