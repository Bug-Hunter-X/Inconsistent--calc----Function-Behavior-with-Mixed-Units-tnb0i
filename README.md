# Inconsistent `calc()` Function Behavior with Mixed Units in CSS

This repository demonstrates a subtle bug related to the use of the `calc()` function in CSS when combining percentage and pixel units.  Certain browsers exhibit unexpected behavior when calculating the final value, potentially leading to layout inconsistencies.

## Bug Description

The core issue lies in how some browsers interpret and perform calculations within the `calc()` function when mixed unit types (percentage and pixels) are used. This can result in incorrect widths or other unexpected rendering behaviors, especially when the parent container's dimensions are smaller than what the calculation suggests.

## Bug Reproduction

1. Clone this repository.
2. Open `bug.html` in different browsers (e.g., Chrome, Firefox, Safari).
3. Observe the width of the `.element` div.  Inconsistencies across browsers highlight the bug.

## Solution

The solution, demonstrated in `bugSolution.css`, involves avoiding mixing units in `calc()` whenever possible. Using a consistent unit type for both values ensures more consistent rendering across different browsers.