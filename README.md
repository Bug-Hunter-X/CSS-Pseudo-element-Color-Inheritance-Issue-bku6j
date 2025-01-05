# CSS Pseudo-element Color Inheritance Bug

This repository demonstrates a subtle bug related to CSS pseudo-element color inheritance.  In certain circumstances, a pseudo-element (specifically `::before` in this example) may fail to inherit the `color` property from its parent element.

The issue is inconsistent across different browsers and CSS configurations, making it difficult to diagnose and fix.

## Problem Description

The `bug.css` file contains CSS code where the `::before` pseudo-element is *expected* to inherit the blue color from its parent. However, it might render in a different color (e.g., black), depending on the browser and other CSS rules in effect.

## Solution

The `bugSolution.css` file offers a solution to ensure consistent color inheritance.  This typically involves explicitly specifying the color property on the pseudo-element itself, overriding any potential inconsistencies.

## Reproduction

1. Clone this repository.
2. Open `index.html` (you'll need to create a very simple HTML file referencing bug.css and bugSolution.css) in your browser.
3. Observe the difference in color rendering between the original and fixed versions.

This example highlights the importance of explicit styling and thorough browser testing when working with CSS pseudo-elements.