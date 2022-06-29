# Read 5 - What is CSS

## CSS:

1. Can be written in three ways:
    - Internally
    - inline
    - externally

2. The dev tools in chrome are critical to understanding what is happening on a page’s styling.

3. Using a CSS Reset is a best practice to reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, etc. The basic reason is that all browsers have presentation defaults, but no browsers have the same defaults.   For example, some browsers indent unordered and ordered lists with left margins, whereas others use left padding. 

## CSS is a rule-based language:
You define the rules by specifying groups of styles that should be applied to particular elements or groups of elements on your web page.


1. The CSS rule opens with a selector . This selects the HTML element that we are going to style. 
2. We then have a set of curly braces { }.
3. Inside the braces will be one or more declarations, which take the form of property and value pairs. CSS properties have different allowable values, depending on which property is being specified. 

## Three ways of inserting a style sheet:
1. External CSS: With an external style sheet, you can change the look of an entire website by changing just one file. Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section. An external style sheet can be written in any text editor, and must be saved with a .css extension. The external .css file should not contain any HTML tags.
 
2. Internal CSS: An internal style sheet may be used if one single HTML page has a unique style. The internal style is defined inside the <style> element, inside the head section.
 
3. Inline CSS: An inline style may be used to apply a unique style for a single element. To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

## Multiple Style Sheets
If some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used. What style will be used when there is more than one style specified for an HTML element?

All the styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

1. Inline style (inside an HTML element)
2. External and internal style sheets (in the head section)
3. Browser default

So, an inline style has the highest priority, and will override external and internal styles and browser defaults.
