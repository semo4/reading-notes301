# Responsive Web Design
![images](images/r.jpg)

## Definition 
- Responsive means that we can create web page that can display in each device (Pc, Laptop, Tablet, Mobile)
no matter the screen size 

## Responsive vs. Adaptive vs. Mobile
![images](images/r2.jpg)
### Responsive
- means to react quickly and positively to any change
### Adaptive
-  means to be easily modified for a new purpose or situation
### Mobile
- means to build a separate website commonly on a new domain solely for mobile users


*there are three main component in responsive web design *
1. *flexible layouts* can resize to any width
2.  *media queries* ability to specify different styles for individual browser and device circumstances
3. *flexible media* equally important aspect to responsive web design


# Float
## Definition 
- Float is a CSS positioning property
- floats can be used to create entire web layouts.
- Floats are also helpful for layout in smaller instances.

## Clearing the Float
- Clear has four valid values as well. 
    1. *Both* clears floats coming from either direction
    2. *Left and Right* can be used to only clear the float from one direction respectively
    3. *Inherit* 
    4. *None* is the default
- we can clear float be using the syntax
    - `clear: both;`

## Problems with Floats
1. **Pushdown** : the items maybe be wider than float  itself 
2. **Double Margin Bug** : if you apply a margin in the same direction as the float, it will double the margin. 
3. **The 3px Jog** :  is when text that is up next to a floated element is mysteriously kicked away by 3px like a weird forcefield around the float
4. **Bottom Margin Bug** :  is when if a floated parent has floated children inside it, bottom margin on those children is ignored by the parent.
