# Javascript Templating Language and Engine— Mustache.js with Node and Express
- We use template to render client-side with javaScript using Json Data
- The template is HTML markup
- The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.

# Mustache
- is a logic-less template syntax
- It can used for :
    1. HTML
    2. config files
    3. source code
- It is often referred to as “logic-less” because there are no if statements
- else clauses, or for loops. Instead, there are only tags
- mustache.js is an implementation of the mustache template system in JavaScript
- mustache supports various languages
- we can use placeholder in mustache by provide {{ name }}

## Mustache-Express
- we use mustache with Node and Express
- to install it: 
    - With Yarn:
        - $ yarn add mustache-express
    -  with NPM:
        - $ npm install mustache --save

# Flexbox
## Properties for the Parent (flex container)
1. **display**
    - This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
2. **flex-direction**
    - This establishes the main-axis, thus defining the     direction flex items are placed in the flex container  it take four value:

      
3. **flex-wrap**
    - By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.


4. **flex-flow**
    - This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.

5. **justify-content**
   - This defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.

6. **align-content**
    - This aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis.
## Properties for the Children (flex items)
1. **order**
    - By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.
2. **flex-grow**
    - This defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up
3. **flex-shrink**
    - This defines the ability for a flex item to shrink if necessary.
4. **flex-basis**
    - This defines the default size of an element before the remaining space is distributed.
5. **flex**
    - This is the shorthand for flex-grow, flex-shrink and flex-basis combined.
6. **align-self**
    - This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items

