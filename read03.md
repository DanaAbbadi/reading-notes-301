# Javascript Templating Language and Engine— Mustache.js with Node and Express

### Javascript Templating

JavaScript templating refers to the client side data binding method implemented with the JavaScript language. 
This approach became popular thanks to JavaScript’s increased use, its increase in client processing 
capabilities, and the trend to outsource calculus to the client’s web browser. Popular JavaScript 
templating libraries are **AngularJS**, **Backbone.js**, **Ember.js**, **Handlebars.js**, and ***Mustache.js***. 

The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.


### Mustache

Mustache can be used for HTML, config files, source code - anything. It works by expanding tags in a template using values provided in a hash or object.

We call it "logic-less" because there are no if statements, else clauses, or for loops. Instead there are only tags. Some tags are replaced with a value, some nothing, and others a series of values. This document explains the different types of Mustache tags.


Tags are indicated by the double mustaches. {{person}} is a tag, as is {{#person}}. In both examples, we'd refer to person as the key or tag key.

If you intend you use mustache with Node and Express, you can use mustache-express. Mustache Express lets you use Mustache and Express together easily.

mustache.js is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating.


# Flexbox

Flexbox is a one-dimensional layout method for laying out items in rows or columns. Items flex to fill additional space and shrink to fit into smaller spaces. In other words, Flexbox Layout aims at providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and/or dynamic.

### Properties for the Parent (flex container)

![container](https://css-tricks.com/wp-content/uploads/2018/10/01-container.svg)

   * ***display***
     
     This defines the parent as a flex container

     ```
     .container {
          display: flex; /* or inline-flex */
      }

      ```

   * ***flex-direction***
     To establishe the main-axis.

     ```
     .container {
        flex-direction: row | row-reverse | column | column-reverse;
      }

     ```  
     - *row* (default): left to right in ltr; right to left in rtl
     - *row-reverse*: right to left in ltr; left to right in rtl
     - *column*: same as row but top to bottom
     - *column-reverse*: same as row-reverse but bottom to top

   * ***flex-wrap***
      
      ![flex-wrap](https://css-tricks.com/wp-content/uploads/2018/10/flex-wrap.svg)
      By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.

     ```
      .container {
         flex-wrap: nowrap | wrap | wrap-reverse;
       }
     ```


     - *nowrap* (default): all flex items will be on one line
     - *wrap*: flex items will wrap onto multiple lines, from top to bottom.
     - *wrap-reverse*: flex items will wrap onto multiple lines from bottom to top.




   * ***flex-flow***

     This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.

     ```
     .container {
        flex-flow: column wrap;
      }
     ```
       


### Properties for the Children (flex items)

![items](https://css-tricks.com/wp-content/uploads/2018/10/02-items.svg)

   * ***order***
     By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.

     ```
     .item {
       order: 5; /* default is 0 */
     }
     ```


   * ***flex-grow***

     This defines the ability for a flex item to grow if necessary. If all items have flex-grow set to 1, the remaining space in the container will be distributed equally to all children.

     ```
     .item {
        flex-grow: 4; /* default 0 */
      }
     ```

   * ***flex-shrink***
    
     This defines the ability for a flex item to shrink if necessary.

     ```
     .item {
       flex-shrink: 3; /* default 1 */
     }
     ```

   * ***flex-basis***

     This defines the default size of an element before the remaining space is distributed. The auto keyword means “look at my width or height property”:

     ```
     .item {
        flex-basis:  | auto; /* default auto */
      }
      ```

   * ***flex***
     
     This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. The default is 0 1 auto, but if you set it with a single number value, it’s like 1 0.

     ```
     .item {
       flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]
     }
     ```

     









