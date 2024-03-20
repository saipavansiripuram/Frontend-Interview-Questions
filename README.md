
# Frontend Interview Questions 

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


### 3. Explain React LifeCycle 

![PVPr1dK](https://github.com/saipavansiripuram/Frontend-Interview-Questions/assets/69411783/7b95a48a-1201-4daf-86bf-aab1159e2aa7)



 React has several lifecycle methods that are invoked at different stages of a component's existence. These methods can be categorized into three phases: Mounting, Updating, and Unmounting. Here's an explanation of each phase along with the corresponding lifecycle methods:

### Mounting Phase:
1. **constructor()**: This is the first method called when a component is initialized. It's used for initializing state and binding event handlers.
   
2. **render()**: This method is responsible for rendering the component's UI based on its current state and props. It must be pure, meaning it should not modify component state or interact with the DOM directly.

3. **componentDidMount()**: This method is invoked immediately after the component is mounted (inserted into the DOM). It's commonly used for performing side effects such as fetching data from an API or interacting with the DOM.

### Updating Phase:
4. **static getDerivedStateFromProps()**: This static method is invoked right before rendering when new props or state are received. It returns an object to update the state, or null to indicate no changes are needed. It's rarely used in favor of componentDidUpdate or shouldComponentUpdate.

5. **shouldComponentUpdate()**: This method allows you to control whether the component should re-render or not. It returns true if the component should update and false otherwise, based on the comparison of current and next props/state.

6. **render()**: Same as the mounting phase, render() is called to re-render the updated UI based on the new state and props.

7. **getSnapshotBeforeUpdate()**: This method is invoked right before the rendered output is committed to the DOM. It allows the component to capture some information from the DOM (e.g., scroll position) before it potentially changes.

8. **componentDidUpdate()**: This method is invoked immediately after the component is updated and re-rendered. It's used for performing side effects like making network requests based on changes in props or state.

### Unmounting Phase:
9. **componentWillUnmount()**: This method is called immediately before a component is unmounted and destroyed. It's used for cleanup tasks such as cancelling network requests, removing event listeners, or clearing timers.

### Error Handling:
10. **static getDerivedStateFromError()**: This static method is invoked after an error has been thrown by a descendant component. It allows the component to update its state in response to the error.

11. **componentDidCatch()**: This method is called after an error has been thrown by a descendant component. It's used to log the error information or perform fallback UI rendering.

These lifecycle methods provide developers with hooks to execute code at specific stages of a component's lifecycle, enabling them to manage state, perform side effects, and handle errors effectively. However, it's important to note that some lifecycle methods have been deprecated or will be deprecated in future releases of React, so it's essential to refer to the official React documentation for the most up-to-date information.

### 3. Explain Angular LifeCycle 

# Angular Lifecycle Hooks

![hooks-in-sequence-f0284a4e9a015ae19cb006fb53e006090cc53291cd6c0ab434ec8494f8ba4af3](https://github.com/saipavansiripuram/Frontend-Interview-Questions/assets/69411783/13313004-d5b6-4d07-8c88-afdb01ff49cf)


Creation: When a component is created, Angular sets it up and initializes any data it needs.

Updates: As the application runs, data might change, triggering updates to the component. Angular keeps track of these changes and updates the component accordingly.

Rendering: After the component is set up and updated, Angular renders it on the screen, showing the user what they need to see.

Destruction: Eventually, the component may no longer be needed. Angular cleans it up and removes it from the application.

Angular provides a set of lifecycle hooks that allow you to tap into the component's lifecycle and perform certain actions at specific points. These hooks can be categorized into four main categories: Initialization, Content Projection, Content Initialization, and Destruction.

## Initialization

### ngOnChanges
- Invoked whenever one or more input properties of the component change.
- It receives a SimpleChanges object containing the previous and current values of the input properties.

### ngOnInit
- Invoked once after the first ngOnChanges.
- Used for initializing the component, such as fetching initial data from a service.

## Content Projection

### ngAfterContentInit
- Invoked once after the component's content has been projected into its view.
- Used for initialization that relies on content projection, such as querying projected content.

### ngAfterContentChecked
- Invoked after every check of the component's projected content.
- Used for additional checks or actions after the content has been projected.

## Content Initialization

### ngAfterViewInit
- Invoked once after the component's view (and child views) have been initialized.
- Used for initializing the component's view or interacting with its child views.

### ngAfterViewChecked
- Invoked after every check of the component's view (and child views).
- Used for additional checks or actions after the view has been initialized.

## Destruction

### ngOnDestroy
- Invoked just before the component is destroyed and removed from the DOM.
- Used for cleanup tasks such as unsubscribing from observables or clearing timers.

## Example Usage:

```typescript
import { Component, OnInit, OnDestroy } from '@angular/core';

@Component({
  selector: 'app-example',
  templateUrl: './example.component.html',
  styleUrls: ['./example.component.css']
})
export class ExampleComponent implements OnInit, OnDestroy {

  constructor() { }

  ngOnInit(): void {
    // Initialization logic here
  }

  ngOnDestroy(): void {
    // Cleanup logic here
  }

}

In Angular, the lifecycle hooks are methods that Angular calls at certain points in the lifecycle of a component or directive. These hooks allow you to perform actions at specific moments, such as initialization, change detection, content projection, and destruction of the component or directive.

Here's a brief overview of the lifecycle hooks in Angular:

1. *ngOnChanges():* This hook is called when Angular detects changes to input properties of the component or directive. It receives a SimpleChanges object that contains the previous and current values of the input properties.

2. *ngOnInit():* This hook is called after Angular has initialized all data-bound properties of a directive or component. It is a good place to perform initialization tasks, such as fetching data from a server.

3. *ngDoCheck():* This hook is called during every change detection cycle, allowing you to implement custom change detection logic. It is called more frequently than ngOnChanges() and is often used for performance optimization.

4. *ngAfterContentInit():* This hook is called after Angular projects external content into the component's view, such as child components or projected content. It is a good place to perform initialization tasks related to content projection.

5. *ngAfterContentChecked():* This hook is called after Angular checks the content projected into the component. It is called every time the projected content changes.

6. *ngAfterViewInit():* This hook is called after Angular initializes the component's view and child views (if any). It is a good place to perform initialization tasks related to the view.

7. *ngAfterViewChecked():* This hook is called after Angular checks the component's view and child views (if any). It is called every time the view or child views change.

8. *ngOnDestroy():* This hook is called just before Angular destroys the component or directive. It is a good place to clean up resources, such as unsubscribing from observables or removing event listeners.

By implementing these lifecycle hooks in your components or directives, you can control and manage their behavior throughout their lifecycle, ensuring proper initialization, change detection, and cleanup.

