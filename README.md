# Frontend-Interview-Questions

# Web Development Interview Questions and Answers

## HTML:

### 1. What is HTML?
HTML stands for HyperText Markup Language. It's the standard markup language used to create and design web pages.

### 2. What is the difference between a tag and an element?
Tags are individual components of HTML that define specific elements, while elements refer to the entire structure defined by the opening and closing tags, along with the content within them.

### 3. What are semantic elements?
Semantic elements in HTML are those that provide meaning to the content they encapsulate, aiding in better structuring and understanding of the document. Examples include `<header>`, `<footer>`, `<nav>`, `<article>`, etc.

### 4. What are attributes?
Attributes are additional information provided within HTML tags to modify or define the behavior or appearance of the element. They are typically in the form of name-value pairs.

### 5. What is the difference between `<div>` and `<span>`?
`<div>` and `<span>` are both HTML elements used for grouping content, but `<div>` is a block-level element, meaning it takes up the full width available, while `<span>` is an inline element, meaning it only takes up the space necessary for its content.

### 6. Can you give examples of inline elements?
Examples of inline elements include `<span>` and `<img>`.

### 7. Besides width, what is another difference between block and inline elements?
Block-level elements start on a new line, whereas inline elements do not.

### 8. Can inline elements have height and width specified?
Generally, inline elements do not have specified height and width, but certain replaced inline elements like `<img>` can have predefined dimensions.

### 9. Do you know the difference between CANVAS & SVG?
Yes, CANVAS and SVG are both used for drawing graphics on web pages, but they have different underlying technologies and methods of rendering. CANVAS uses a raster-based approach, while SVG is vector-based.

## CSS:

### 1. What is the full form of CSS?
CSS stands for Cascading Style Sheets.

### 2. What is cascading in CSS?
Cascading refers to the process of determining which styles should be applied to an element when multiple conflicting styles exist. Styles are applied based on specificity and the order of appearance.

### 3. What is specificity?
Specificity in CSS determines which style rule is applied when multiple rules conflict. It's based on the selector's specificity value.

### 4. What is the default value of the position property?
The default value of the position property in CSS is "static".

### 5. What is the difference between position relative and position absolute?
Position relative positions an element relative to its normal position, while position absolute positions an element relative to its nearest positioned ancestor.

### 6. What is flexbox?
Flexbox is a layout system in CSS that allows for the easy alignment and distribution of elements within a container along a single axis or across multiple axes.

### 7. What is the box model?
The box model in CSS refers to the way elements are structured, consisting of content, padding, border, and margin.

### 8. What is the difference between content box and border box?
Content box includes only the content of an element, while border box includes the content, padding, and border.

### 9. What is the difference between margin and padding?
Margin is the space around an element, while padding is the space between the content and the border of an element.

## JavaScript:

### 1. Why do you need JavaScript for web pages?
JavaScript is essential for web pages because it adds interactivity and dynamic behavior to otherwise static HTML and CSS.

### 2. What are the data types in JavaScript?
JavaScript has eight primitive data types and seven non-primitive (or reference) data types.

### 3. What is meant by primitive?
Primitive data types are basic data types that are immutable and directly stored in memory.

### 4. How many ways can we create variables in JavaScript?
Variables in JavaScript can be created using var, let, or const keywords.

### 5. What is the difference between let and var?
The main difference between let and var is that var is function-scoped, while let is block-scoped.

### 6. What is the difference between parameters and arguments?
Parameters are variables in a function definition, while arguments are the actual values passed to the function when it is invoked.

### 7. What is the difference between slice and splice methods?
The difference between slice and splice methods in JavaScript is that slice returns a new array containing elements selected from the original array, while splice changes the contents of an array by removing or replacing existing elements.

### 8. What are MAP, Filter, and Reduce used for?
MAP, Filter, and Reduce are higher-order array methods used for transforming or manipulating arrays.

### 9. What are promises in JavaScript?
Promises in JavaScript represent the eventual completion or failure of an asynchronous operation, allowing for better handling of asynchronous tasks.

### 10. What is the DOM?
DOM (Document Object Model) is a tree-like structure representing the elements of an HTML document, enabling interaction and manipulation of the document content.

### 11. What is event bubbling and event capturing?
Event bubbling and event capturing are two different ways of event propagation in the DOM, where events are either propagated from the innermost element up to the outermost (bubbling) or from the outermost element down to the innermost (capturing).

## React:

### 1. Why do we need React?
React is needed because it simplifies the process of building complex user interfaces by providing component-based architecture and efficient state management, enhancing code maintainability and reusability compared to plain JavaScript.

### 2. What is the difference between imperative and declarative programming in React?
Imperative programming focuses on how to achieve a result by specifying each step, while declarative programming focuses on what result is desired without specifying how to achieve it, letting the framework handle the implementation details. React encourages a more declarative approach to building UIs.
