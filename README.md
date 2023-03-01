# MERN-Question-Bank

### 1. What is the difference between flex and grids?

Flexbox and Grid are both CSS layout modules used to design and structure web pages, but they have some key differences.

Flexbox is a one-dimensional layout module that focuses on arranging items within a container in a linear direction, either horizontally or vertically. It is best suited for laying out small sections of a web page, such as navigation menus or individual components. Flexbox is particularly useful for responsive design, as it allows for easy reordering and alignment of items on different screen sizes.

On the other hand, CSS Grid is a two-dimensional layout module that enables designers to create complex and responsive layouts. It allows for precise placement of elements in rows and columns, creating a flexible grid system. CSS Grid is ideal for larger sections of a web page, such as the main content area, and it can handle both row-based and column-based layouts.

In summary, while Flexbox is a powerful tool for arranging elements in a single direction, CSS Grid offers more flexibility and control over layout design in both dimensions. The choice between Flexbox and CSS Grid will depend on the specific design needs of the project at hand.

---

### 2. Give an example where we have to use grids and where you have to use flexbox?
Example of using CSS Grid:
Let's say you have a complex layout with multiple rows and columns, where you want to position elements precisely in specific cells or regions of the grid. In this case, you could use CSS Grid to create a flexible grid system that allows you to define rows and columns, set the size of grid areas, and place elements exactly where you want them. For instance, you might use CSS Grid to create a responsive dashboard with multiple widgets, each occupying a specific region of the grid, with the ability to rearrange them based on the screen size.

Example of using Flexbox:
On the other hand, suppose you have a simple layout where you want to align items along a single axis, such as a horizontal navigation menu or a row of cards. In this case, you could use Flexbox to create a flexible and responsive layout that automatically adjusts to different screen sizes. With Flexbox, you can easily center, space, and order items along the main axis, making it an ideal choice for creating small, single-directional layouts that require a high degree of flexibility. For instance, you might use Flexbox to create a responsive gallery with images aligned horizontally, with the ability to wrap them onto multiple rows as needed.

---

### 3. What does @media do?

@media is a CSS rule that allows designers to specify different styles for different screen sizes or devices. It is used to create responsive web pages that adapt to the user's device, whether it's a desktop computer, tablet, or smartphone.

The @media rule works by defining a set of CSS rules that apply only when a certain condition is met. The condition is based on the media type or media features, such as screen size, resolution, orientation, and color scheme. For example, you might use @media to define a different font size for mobile devices compared to desktop devices, or to hide certain elements on small screens to improve readability.

---

### 4. What are the differences between relative and absolute in CSS?

In CSS, relative and absolute are two positioning schemes used to position elements on a web page. The key differences between relative and absolute positioning are:

#### Relative Positioning:

It positions an element relative to its normal position within the document flow.
The element is moved from its original position, but the space it occupied is still reserved, so other elements will not fill its space.
It can be moved using top, right, bottom, and left properties, which define the offset from its original position.
It can be used for minor adjustments or to create a more complex layout by positioning elements relative to each other.
If the parent element is positioned relative, the child element's position is relative to its parent element.

#### Absolute Positioning:

It positions an element relative to the nearest positioned ancestor (the nearest ancestor element that is positioned).
It removes the element from the document flow, so other elements will fill its space.
It can be moved using top, right, bottom, and left properties, which define the offset from the nearest positioned ancestor.
It can be used to position elements precisely and create overlays or popups that appear above other elements.
If there is no positioned ancestor, the element is positioned relative to the body element.
In summary, relative positioning moves an element from its original position while still reserving its space, while absolute positioning removes an element from the document flow and positions it relative to the nearest positioned ancestor. Both positioning schemes have their specific use cases, and the choice between them depends on the design needs of the project at hand.

---

### 5. What is scoping?

In web development, scoping refers to the concept of limiting the scope or visibility of CSS styles to specific parts of a web page. This can be achieved using various CSS techniques, such as classes, IDs, or pseudo-selectors, to target specific elements or groups of elements.

The main benefit of scoping CSS styles is to avoid unwanted style inheritance and unintended style conflicts. By scoping styles to specific elements, developers can ensure that their styles are only applied to the intended elements, and not to other elements that might share the same selectors. This helps to improve the predictability and maintainability of the code, especially in large and complex projects.

There are several ways to scope CSS styles, including:

Classes: by adding a class attribute to an element, developers can create specific CSS styles that only apply to elements with that class.
IDs: similar to classes, IDs can be used to create specific CSS styles that only apply to elements with that ID.
Pseudo-selectors: these are selectors that target specific parts of an element, such as its first child or hover state.
Descendant selectors: by targeting a specific element within a parent element, developers can scope CSS styles to that particular element and its descendants.
Overall, scoping CSS styles is an important concept in web development that helps to ensure the consistency and predictability of the styling of a web page.

---

### 6. What are closures? Few Common Uses for closures :

In JavaScript, a closure is a combination of a function and the lexical environment in which it was declared. This allows the function to access variables and parameters from its outer scope, even after the outer function has returned. Closures are a powerful feature of JavaScript that enables functional programming techniques and can be used to implement various design patterns.

Here are some common uses for closures in JavaScript:

Private variables: closures can be used to create private variables and methods that are hidden from the global scope. This can help to prevent naming conflicts and improve code maintainability.

Factory functions: closures can be used to create factory functions that return other functions with pre-defined parameters or behavior. This can help to reduce code duplication and improve code reuse.

Memoization: closures can be used to implement memoization, which is a technique for caching the results of expensive function calls. By caching the results of a function call, subsequent calls can be returned from the cache instead of recomputing the result.

Event handlers: closures can be used to create event handlers that have access to the event object and other variables in the outer scope. This can help to simplify event handling code and improve code organization.

Iterators and generators: closures can be used to implement iterators and generators, which are functional programming techniques for processing collections of data. By using closures to store the state of the iteration, these techniques can be used to implement lazy evaluation and improve performance.

Overall, closures are a powerful feature of JavaScript that enable functional programming techniques and can be used to improve code maintainability, performance, and organization

---

### 7. Explain promises to a 5 year old, with simple examples

Promises are a way for a computer program to make a promise to do something in the future and then keep that promise.

Let's say you want to get a cookie from your mom, but she's busy right now. She promises to give you a cookie after she finishes her work. This is like a promise in programming - the program promises to do something in the future.

But how do you know when your mom is done with her work and ready to give you the cookie? She might tell you to wait until she's finished, or she might forget about her promise.

In programming, a Promise is like a special note that tells you when the program is done with its work and ready to give you the result. It's a way to keep track of a promise and make sure it's fulfilled.

For example, imagine you're playing a game where you need to find a hidden treasure. You send your computer on a mission to find the treasure, but it might take a while. Instead of waiting for the computer to finish, you give it a Promise to come back and tell you when it's found the treasure. Then you can keep playing the game while the computer works in the background.

When the computer finds the treasure, it comes back and tells you with the Promise. You can then use the treasure in the game to unlock new levels or get special powers.

In summary, Promises are a way for a program to make a promise to do something in the future and then keep that promise by using a special note to notify you when it's done. It's like asking your mom for a cookie and waiting for her to tell you when it's ready, or sending your computer on a mission and getting a notification when it's done.

---

### 8. What is currying?

Currying is a functional programming technique that involves transforming a function that takes multiple arguments into a series of functions that each take a single argument. The resulting functions can be composed together to create more flexible and reusable code.

The name "currying" comes from the mathematician Haskell Curry, who was a pioneer in the field of combinatory logic and functional programming.

In JavaScript, currying can be achieved using the bind() method or by manually creating a closure that returns a new function. Here's an example:

<img width="438" alt="image" src="https://user-images.githubusercontent.com/110287987/222050595-d6eef788-bcbf-4a35-ad69-45d7c6f75c78.png">

In this example, the add() function takes two arguments, but we've created a curried version of it called curryAdd() that takes one argument at a time. We can then use the curryAdd() function to create a new function called addTwo that always adds 2 to its argument. When we call addTwo(3), it returns the result of adding 2 and 3, which is 5.

Currying can be useful in many situations, such as when you want to create a series of functions with similar behavior but different parameters, or when you want to create higher-order functions that take other functions as arguments. It can also help to simplify and modularize code, making it easier to understand and maintain.

---
