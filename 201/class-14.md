# Class 14a / 14b Reading

# What Google Learned From Its Quest to Build the Perfect Team
- the whole artical was talk about the teams and how we can know the successful teams.
- I had read all of it and I have some thought about the team work:
1. to create good team give them chance to communicate with each other to make there connection with each other.
2. give all team member chance to talk and explain ther ideas.
3. It should be between them recpect.
4. also It should be between them the responsability for the team.
5. the final thing is it must supported each other and try to share the thought.

# Transforms
- the Transform property in css give us the ability to modify the position os the element.
- there are two value for Transform: 
    1. two-dimensional
    2. three-dimensional

## Transform Syntax
- there is multiple syntax for each browsre:
    1. we use to chrome: -webkit-transform
    2. we use to firefox: -moz-transform
    3. we use for all browsre : transform

## 2D Transforms
- it take multiple property
### 1.  2D Rotate
- with this proparty we can rotate the element from 0 to 360 degree.
    - syntex : transform: rotate(20deg);
- it can also take percentage value and negative value


### 2. 2D Scale
- this property allow us to change the size of any element it take fraction number .
    - syntax : transform: scale(.75);
- we can spicify the scale on one of the axis  x or y
    - syntax : transform: scaleX(.5);

    - syntax : transform: scaleY(1.15);

### 3. 2D Translate
- this property allow us to change the position of element 
- it can by in three value 
    1. on y axis : transform: translateX(-10px);
    2. on x axis : transform: translateY(25%);
    3. on both deriction :transform: translate(-10px, 25%);
- it can take many type of value : 
    1. percentage value
    2. pixels value
    3. negative value
- the element  will by move by two deriction by the value
    1. Positive 
        - it will push the element to down and right
    2. negative 
        - it will push the element to up and left

    
### 4. 2D Skew
- it distort elements on three way
    1. horizontal axis : transform: skewX(5deg);
    2. vertical axis : transform: skewY(-20deg);
    3. or both : transform: skew(5deg, -20deg);
- it take only one value that is degree
- it tale negative and posative value 
- it dose not execpt pixle and percentage value

## Combining Transforms
- it allow us to concatenat between the Transforms that mean we can use the  Transforms in same statment 
     - transform: rotate(25deg) scale(.75);
     - transform: skew(10deg, 20deg) translateX(20px);


# Transform Origin
- we use it to change the default position value of any element
    - syntax it take four vakue : 
        1.  transform-origin: 0 0;
        2. transform-origin: 100% 100%;
        3. transform-origin: top left;
        4. transform-origin: 20px 50px;
- there is one case that we can give it one value and it will take it for both horizontal and vertical axes

# Perspective
- we use it to make element seen in three-dimensional drawings.

# 3D Transforms
- in 3D Transforms we will work with three axis x,y and z 

### 1. 3D Rotate
- in this propertyr we can rotate any element around any axes 
- the value that can take is rotateX, rotateY, and rotateZ.
- syntax:
      - transform: perspective(200px) rotateX(45deg);
      - transform: perspective(200px) rotateY(45deg);
      - transform: perspective(200px) rotateZ(45deg);

### 2. 3D Scale
- we can use only one value it is scaleZ
- syntax :  transform: perspective(200px) scaleZ(.25) rotateX(45deg);

### 3. 3D Translate
- it take one value also on z axis and it not take value on x, y axis
- syntax :  transform: perspective(200px) translateZ(50px);

### 4. 3D Skew
- it cannot  transform on three-dimensional scale



# Transitions & Animations
##  Transitions
- it is the ability to make elemnt to change it is state to another
- we can use different state and we call it pseudo-classes.:
    1. :hover
    2. :focus
    3. :active
    4. :target 
- for the transition ther are four property we can use :
1. transition-property
2. transition-duration
3. transition-timing-function
4. transition-delay.

### transition-property
- we use it to determine what property we will want to change
- syntax : transition-property: background
- here we want the change on background

### transition-duration
- we determine the time to do the change 
- syntax : transition-duration: 1s;
- we can use two value for it second and millisecond


### transition-timing-function
- we determine the type of change 
- syntax :  transition-timing-function: linear;
- it take four value: 
    1. linear
    2. ease-in
    3. ease-out
    4. ease-in-out.

### transition-delay.
- it determine the time before the change execut.
- it take two value seconds or milliseconds
- syntax : transition-delay: 0s, 1s;

## Transitional Properties
- not all properties may be transitioned
- we can use transition on this property:
    - background-color
    - background-position
    - border-color
    - border-width
    - border-spacing
    - bottom
    - clip
    - color
    - crop
    - font-size
    - font-weight
    - height
    - left
    - letter-spacing
    - line-height
    - margin
    - max-height
    - max-width
    - min-height
    - min-width
    - opacity
    - outline-color
    - outline-offset
    - outline-width
    - padding
    - right
    - text-indent
    - text-shadow
    - top
    - vertical-align
    - visibility
    - width
    - word-spacing
    - z-index

# Animations
- we use it to allow the element move from state to state in sequance 
### Animations Keyframes
- we use the animation name and give it multiple vlaue to determin how it move
- syntax : animation-name: slide;
- after we use the animation name we use the @keyframes keyword to give the name it is movement 
- syntax :
    - ` @keyframes slide {`
              `0% {`
                   ` left: 0;`
                  `  top: 0;`
              `  }`
                `50% {`
                 `   left: 244px;`
                   ` top: 100px;`
              `  }`
               ` 100% {`
                  ` left: 488px;`
                   ` top: 0;`
                `}`
               ` }`


