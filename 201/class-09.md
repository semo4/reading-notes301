# Class 09 Reading

# HTML
## Chapter 7 Forms

- the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.
- form can make us to collect information from users or visiters.

### Why Forms?
 - The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage.

### Form Controls
- there are four type of form control. 
1. ADDING TEXT:
    - Text input (single-line)
    Used for a single line of text such
    as email addresses and names.
    - Password input
    Like a single line text box but it
    masks the characters entered.
    - Text area (multi-line)
    For longer areas of text, such as
    messages and comments.
2. Ma king Choices:
    - Radio buttons
    For use when a user must select
    one of a number of options.
    - Checkboxes
    When a user can select and
    unselect one or more options.
    - Drop-down boxes
    When a user must pick one of a
    number of options from a list.
3. Submitting Forms:
    - Submit buttons
    To submit data from your form
    to another web page.
    - Image buttons
    Similar to submit buttons but
    they allow you to use an image.
4. Uploading Files:
    - File upload
    Allows users to upload files
    (e.g. images) to a website.

### Form Structure
- **form**
    Form controls live inside a
    `<form>` element. This element
    should always carry the action
    attribute and will usually have a
    method and id attribute too.
- **action**
    Every `<form>` element requires
    an action attribute. Its value
    is the URL for the page on the
    server that will receive the
    information in the form when it
    is submitted.
- **method**
    Forms can be sent using one of
    two methods: get or post.


### Text Input
- there is multiple text input we can use
- **input**
    The `<input>` element is used
    to create several different form
    controls. The value of the type
    attribute determines what kind
    of input they will be creating.
- **type**
    - it take multi value: 
    1. **type="text"**
    When the type attribute has a
        value of text, it creates a singleline
        text input.
    2. **type="password"** 
    When the type attribute has
    a value of password it creates
    a text box that acts just like a
    single-line text input, except
    the characters are blocked out.
    3. **type="radio"** 
    Radio buttons allow users to pick
    just one of a number of options.
    4. **type="checkbox"**
    Checkboxes allow users to select
    (and unselect) one or more
    options in answer to a question.
    5. **type="file"**
    This type of input creates a
    box that looks like a text input
    followed by a browse button.
    When the user clicks on the
    browse button, a window opens
    up that allows them to select a
    file from their computer to be
    uploaded to the website.
    6. **type="email"**
    When the type attribute has
    a value of email it creates
    a text box that can check the email if it write correctly.
    7. **type="submit"**
    The submit button is used to
    send a form to the server.
    8. **type="image"**
    If you want to use an image for
    the submit button
    9. **type="hidden"**
    This example also shows a
    hidden form control. These form
    controls are not shown on the
    page
    10. **type="date"**
    If you are asking the user for a
    date, you can use an `<input>`
    element and give the type
    attribute a value of date.
    This will create a date input in
    browsers that support the new
    HMTL5 input types.
    11. **type="url"**
    A URL input can be used when
    you are asking a user for a web
    page address.
    12. **type="search"**
    If you want to create a single
    line text box for search queries,
    HTML5 provides a special
    search input.
- we can use with input placeholder and name for each type.


### Labelling Form Controls
- **Label** : to descripe the form input .
- there two way to use it:
    1. Wrap around both the text
    description and the form input
    (as shown on the first line of the
    example to your right).
    2. Be kept separate from the
    form control and use the for
    attribute to indicate which form
    control it is a label for (as shown
    with the radio buttons).

- **for** The for attribute states which
form control the label belongs to.

### Grouping Form Elements
- **fieldset**
You can group related form
controls together inside the
`<fieldset>` element. This is
particularly helpful for longer
forms.
- **legend**
The `<legend>` element can
come directly after the opening
`<fieldset>` tag and contains a
caption which helps identify the
purpose of that group of form
controls.

### Form Validation
- Validation helps ensure the
user enters information in a
form that the server will be able
to understand when the form
is submitted.
- Validating the
contents of the form before it is
sent to the server the helps:
1. Reduce the amount of work
the server has to do
2. Enables users to see if there
are problems with the form
faster than if validation were
performed on the server.


# Summary
- Whenever you want to c XX ollect information from
visitors you will need a form, which lives inside a
`<form>` element.
-  Information from a form is sent in name/value pairs.
- Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.
- HTML5 introduces new form elements which make it
easier for visitors to fill in forms.


# CSS
# Chapter 14 Lists, Tables & Forms
### Bullet Point Styles
#### list-style-type
- The list-style-type property
allows you to control the shape
or style of a bullet point (also
known as a marker).
- we can use it with two type of list:
    1. ordered list
    2. unordered list
- **Unordered Lists**
    - For an unordered list you can use
        the following values:
        - none
        - disc
        - circle
        - square
- **Ordered Lists**
    - For an ordered (numbered) list
    you can use the following values:
       - decimal
            - 1 2 3
       - decimal-leading-zero
            - 01 02 03
       - lower-alpha
            - a b c
       - upper-alpha
            - A B C
       - lower-roman
            - i. ii. iii.
       - upper-roman
            - I II III

### Images for Bullets
#### list-style-image
- You can specify an image to act
as a bullet point using the
list-style-image property.

### Positioning the Marker
#### list-style-position
- This property can take one of
    two values:
    - outside
    The marker sits to the left of the
    block of text. (This is the default
    behaviour if this property is not
    used.)
    - inside
    The marker sits inside the box of
    text (which is indented).

### List Shorthand
#### list-style
- it allows you to express
the markers' style, image and
position properties in any order.

### Table Properties
- there are many property to use: 
- **width** to set the width of the
table
- **padding** to set the space
between the border of each table
cell and its content
- **text-transform** to convert the
content of the table headers to
uppercase
- **letter-spacing, font-size**
to add additional styling to the
content of the table headers
- **border-top, border-bottom**
to set borders above and below
the table headers
- **text-align** to align the writing
to the left of some table cells and
to the right of the others
- **background-color** to change
the background color of the
alternating table rows
- **:hover** to highlight a table row
when a user's mouse goes over it

#### styling tables
- **Give cell s padding**
    - Adding padding helps to
    improve readability.
- **Distinguish headings**
    - You can also
    make headings uppercase and
    then either add a background
    color or an underline to clearly
    distinguish them from content.
- **Shade alternate rows**
    - Shading every other row can
    help users follow along the lines.
    Use a subtle distinction from the
    normal color of the rows to keep
    the table looking clean.
- **Align numerals**
    - You can use the text-align
    property to align the content
    of any column that contains
    numbers to the right

### Border on Empty Cells
#### empty-cells
- If you have empty cells in
your table, then you can use
the empty-cells property to
specify whether or not their
borders should be shown.
- it can take one of three value: 
    1. show
    This shows the borders of any
    empty cells.
    2. hide
    This hides the borders of any
    empty cells.
    3. inherit
    If you have one table nested
    inside another, the inherit
    value instructs the table cells to
    obey the rules of the containing
    table.

### Gaps Between Cells
#### border-spacing, border-collapse
- **The border-spacing** property
allows you to control the
distance between adjacent cells.

- **collapse**
    Borders are collapsed into a
    single border where possible.
    (border-spacing will be
    ignored and cells pushed
    together, and empty-cells
    properties will be ignored.)
- **separate**
    Borders are detached from each
    other. (border-spacing and
    empty-cells will be obeyed.)

# Summary
- In addition to the CSS p XX roperties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.
- List markers can be given different appearances
using the list-style-type and list-style image
properties.
- Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.
- Forms are easier to use if the form controls are
vertically aligned using CSS.
- Forms benefit from styles that make them feel more
interactive.


# JavaScript
# Chapter 6 Events 
- When you browse the web, your browser registers different
types of events. It's the browser's way of saying, "Hey, this
just happened." Your script can then respond to these events.

### DIFFERENT EVENT TYPES
- we have three type of event:
1. **UI EVENTS** Occur when a user interacts with the browser's user interface (UI) rather than the web page
    and it have multiple events:
    - load Web page has finished loading
    - unload Web page is unloading (usually because a new page was requested)
    - error Browser encounters a JavaScript error or an asset doesn't exist
    - resize Browser window has been resized
    - scroll User has scrolled up or down the page

2. **KEYBOARD EVENTS** Occur when a user interacts with the keyboard (see also input event)
     and it have multiple events:
    - keydown User first presses a key (repeats while key is depressed)
    - keyup User releases a key
    - keypress Character is being inserted (repeats while key is depressed)

3. **MOUSE EVENTS** Occur when a user interacts with a mouse. trackpad, or touchscreen
    and it have multiple events:
    - click User presses and releases a button over the same element
    - dbl click User presses and releases a button twice over the same element
    - moused own User presses a mouse button while over an element
    - mouseup User releases a mouse button while over an element
    - mousemove User moves the mouse (not on a touchscreen)
    -mouseover User moves the mouse over an element (not on a touchscreen)
    - mouseout User moves the mouse off an element (not on a touchscreen)

4. **FOCUS EVENTS** Occur when an element (e.g., a link or form field) gains or loses focus

    - focus / focusin Element gains focus
    - blur / focusout Element loses focus

5. **FORM EVENTS** Occur when a user interacts with a form element

    - input Value in any `<input>` or `<textarea>` element has changed (IE9+)
    or any element with the contented i table attribute
    - change Value in select box, checkbox, or radio button changes ( IE9+)
    - submit User submits a form (using a button or a key)
    - reset User clicks on a form's res~t button (rarely used these days)
    - cut User cuts content from a form field
    - copy User copies content from a form field
    - paste User pastes content into a form field
    - select User selects some text in a form field

6. **MUTATION EVENTS** Occur when the DOM structure has been changed by a script To be replaced by mutation observers (see p284)

    - DOMSubtreeModified Change hc;is been made to document
    - DOMNodelnserted Node has been inserted as a direct child of another node
    - DOMNodeRemoved Node has been removed from another node
    - OOMNodelnsertedlntoDocument Node has been inserted as a descendant of another node
    - DOMNodeRemovedFromOocument Node has been removed as a descendant of another node


### THREE WAYS TO BIND AN EVENT TO AN ELEMENT 
- Event handlers let you indicate which event you
are waiting for on any particular element.
There are three types of event handlers.
1. HTML EVENT HANDLERS
2. TRADITIONAL DOM EVENT HANDLERS
3. DOM LEVEL 2 EVENT LISTENERS












