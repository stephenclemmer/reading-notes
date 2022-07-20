# CSS Layout

## Learn CSS - Flexbox

**Flexbox is designed for one-dimensional content. Explain what this means.**
Describing Flexbox as one-dimensional refers to the fact that flexbox processes layouts in one dimension at a time, as a row or column; as opposed to the two-dimensional model of the CSS grid layout, which controls columns and rows together.

**Explain the difference between the main axis and cross axis.**
Main Axis: The main axis is the one set by your flex-direction property. If that is row your main axis is along the row, if it is column your main axis is along the column. Flex items move as a group on the main axis. 

Cross axis: The cross axis runs in the other direction to the main axis, so if flex-direction is row the cross axis runs along the column. You can do two things on the cross axis. You can move the items individually or as a group so they align against each other and the flex container. Also, if you have wrapped flex lines, you can treat those lines as a group in order to control how space is assigned to those lines.


**How can using certain properties of flexbox negatively impact accessibility?**

One should be cautious when using any properties that reorder the visual display away from how things are ordered in the HTML document, as it can negatively impact accessibility. The row-reverse and column-reverse values are a good example of this. The reordering only happens for the visual order, not the logical order. This is important to understand as the logical order is the order that a screen reader will read out the content, and anyone navigating using the keyboard will follow.

## CSS Layout - Flexbox

**What are some advantages of using flexbox over float?**

- Vertically centering a block of content inside its parent.
- Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available.
- Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content.

**How does this topic connect with your long term goals?**

I would like to be able to style webpages so that they are dynamic and beautiful. Flexbox seems like a good tool to help achieve this outcome.
