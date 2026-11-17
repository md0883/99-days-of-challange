# Flexbox Fundamentals
>Overview
Flexbox (Flexible Box Layout) is a CSS layout system designed to make arranging, aligning, and distributing elements easier. It helps developers create responsive layouts without relying on floats or complex positioning techniques.

When Flexbox is applied to a container, all direct child elements become flex items and can be controlled efficiently along a horizontal or vertical axis.

>What is Flexbox?
Flexbox allows elements inside a container to:

Align neatly
Distribute available space
Adjust automatically to different screen sizes
Create modern layouts with less code
>To activate Flexbox:
.container {
  display: flex;
}
>justify-content
The justify-content property controls how items are positioned along the main axis.

For a row layout, this means horizontal alignment.

>Example:

.container {
  display: flex;
  justify-content: center;
}
>Common values:

>flex-start
Items stay at the beginning.
justify-content: flex-start;

>center
Items move to the center.
justify-content: center;

>flex-end
Items move to the end.

justify-content: flex-end;
>space-between
Equal space appears between items.

justify-content: space-between;
>space-around
Items receive space around them.

justify-content: space-around;
>space-evenly
All spacing remains perfectly equal.

justify-content: space-evenly;
>align-items
The align-items property controls alignment across the cross axis.

In a row layout, this means vertical alignment.

>Example:

.container {
  display: flex;
  align-items: center;
}
>Common values:

stretch
Default behavior.

align-items: stretch;
center
Centers items vertically.

align-items: center;
flex-start
Places items at the top.

align-items: flex-start;
flex-end
Places items at the bottom.

align-items: flex-end;
gap
The gap property creates consistent spacing between flex items.

>Example:

.container {
  display: flex;
  gap: 20px;
}
>Benefits of using gap:

Cleaner code
No extra margins needed
Consistent spacing
Better readability
Why Use Flexbox?
>Flexbox is helpful because it:

Simplifies layouts
Reduces CSS complexity
Improves responsiveness
Makes alignment easier
Works well for navigation bars, cards, galleries, and menus
