# Uncommon HTML Bug: Incorrect Element Hiding

This repository demonstrates a subtle bug in HTML related to hiding elements.  The bug involves incorrectly using the `visibility` CSS property instead of `display` to hide an element.  While both properties can hide elements, they have different effects on layout.

## The Bug
The `bug.html` file contains a `div` element that is intended to be hidden.  However, the JavaScript code uses `visibility: hidden;`, which only makes the element invisible while still reserving its space in the layout.  This can lead to unexpected layout issues.

## The Solution
The `bugSolution.html` file demonstrates the correct way to hide an element using `display: none;`.  This removes the element from the layout entirely, preventing layout problems.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.  Observe that the div element is hidden but still affects the layout.
3. Open `bugSolution.html` in a web browser. Observe that the div element is hidden and does not affect the layout.