# Basic DOM Manipulation

![DOM Manipulation](https://via.placeholder.com/728x90.png?text=Basic+DOM+Manipulation+Banner)

This repository contains basic examples of DOM (Document Object Model) manipulation using vanilla JavaScript. These examples are aimed at beginners who want to understand how to interact with and modify HTML elements dynamically.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Examples](#examples)
  - [1. Selecting Elements](#1-selecting-elements)
  - [2. Modifying Elements](#2-modifying-elements)
  - [3. Event Listeners](#3-event-listeners)
  - [4. Creating and Removing Elements](#4-creating-and-removing-elements)

## Introduction

DOM manipulation is a fundamental skill for web developers. This repository includes simple examples that demonstrate how to select, modify, and create HTML elements using JavaScript.

## Prerequisites

To work with these examples, you should have a basic understanding of HTML, CSS, and JavaScript. You will also need a web browser and a text editor to write and run the code.

## Getting Started

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/basic-dom-manipulation.git
    ```
2. Navigate to the project directory:
    ```bash
    cd basic-dom-manipulation
    ```
3. Open `index.html` in your web browser to see the examples in action.

## Examples

### 1. Selecting Elements

Learn how to select elements using methods like `getElementById`, `getElementsByClassName`, `getElementsByTagName`, `querySelector`, and `querySelectorAll`.

```javascript
// Select an element by ID
const header = document.getElementById('header');

// Select elements by class name
const items = document.getElementsByClassName('item');

// Select elements by tag name
const paragraphs = document.getElementsByTagName('p');

// Select a single element using a CSS selector
const main = document.querySelector('#main');

// Select multiple elements using a CSS selector
const links = document.querySelectorAll('.nav-link');
```
### 2. Selecting Elements
Learn how to change the content and style of elements.

```<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modifying Elements</title>
</head>
<body>
    <h1 id="header">Original Header</h1>
    <div id="main">Original Content</div>

    <script>
        // Change the text content of an element
        const header = document.getElementById('header');
        header.textContent = 'Welcome to Basic DOM Manipulation';

        // Change the inner HTML of an element
        const main = document.getElementById('main');
        main.innerHTML = '<p>This is a new paragraph</p>';

        // Change the style of an element
        header.style.color = 'blue';
        header.style.fontSize = '2em';
    </script>
</body>
</html>
```
### 3. Event Listeners
Learn how to add and remove event listeners to handle user interactions.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Event Listeners</title>
</head>
<body>
    <button id="myButton">Click Me</button>

    <script>
        // Add a click event listener to a button
        const button = document.getElementById('myButton');
        button.addEventListener('click', handleClick);

        function handleClick() {
            alert('Button clicked!');
        }

        // Remove the event listener
        // button.removeEventListener('click', handleClick);
    </script>
</body>
</html>
```
### 4. Creating and Removing Elements
Learn how to create new elements and remove existing ones from the DOM.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Creating and Removing Elements</title>
</head>
<body>
    <div id="container"></div>
    <div id="oldDiv">This div will be removed</div>

    <script>
        // Create a new element
        const newDiv = document.createElement('div');
        newDiv.textContent = 'This is a new div';

        // Append the new element to the body
        document.getElementById('container').appendChild(newDiv);

        // Remove an element
        const oldDiv = document.getElementById('oldDiv');
        oldDiv.remove();
    </script>
</body>
</html>
```



