![computer on desk with notes and coffee](https://images.unsplash.com/photo-1453928582365-b6ad33cbcf64?q=80&w=2073&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

# The Anatomy of a CSS Selector

A CSS selector is the first part of a CSS Rule. It is a pattern of elements and other terms that tell the browser which HTML elements should be _selected_ to have the CSS property values inside the rule applied to them. The element or elements which are selected by the selector are referred to as the subject of the selector.

## Basic Selector Types

**_Example of a CSS Rule:_**

```css
/* the h1 is the selector in this CSS Rule */
h1 {
  color: blue;
  background-color: yellow;
}
```

### Type Selectors:

Sometimes referred to as a tag name selector or element selector, as it selects an HTML tag/element in your document.

**_Example:_**

```css
/* adding styling to the body element */
body {
  font-family: sans-serif;
}
```

### Class Selectors:

Case-sensitive class selector starts with a dot (.) character. It will select everything in the document with that class applied to it.

**_Example:_**

```css
/* adding styling to an element with a class of .notebox */
.notebox {
  border: 4px solid #666666;
  padding: 0.5em;
  margin: 0.5em;
}
```

### ID Selectors:

Case-sensitive ID selector begins with a # rather than a dot character, but is used in the same way as a class selector.

**_Example:_**

```css
/* adding styling to an element with the ID of #one */
#one {
  background-color: yellow;
}
```

> NOTE: an ID can be used only once per page, and elements can only have a single id value applied to them.

### Selector Lists:

If you have more than one thing that uses the same CSS then the individual selectors can be combined into a selector list so that the rule is applied to all of the individual selectors.

**_Example:_**

```css
/* both h1 and .special have same CSS rules */
h1,
.special {
  color: blue;
}
```

### Universal Selector:

The universal selector is indicated by an asterisk (\*). It selects everything in the document.

It \* is chained using a descendant combinator, it selects everything inside that ancestor element.

**_Example:_**

```css
/* p * selects all the nested elements inside the <p> element */
p * {
  margin: 0;
}
```

For more information on CSS selectors and how they are used, check out the MDN docs.
[MDN Docs](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Basic_selectors)
