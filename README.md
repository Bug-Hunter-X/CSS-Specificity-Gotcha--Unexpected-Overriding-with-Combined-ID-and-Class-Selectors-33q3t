# CSS Specificity Gotcha: Unexpected Overriding with Combined ID and Class Selectors

This repository demonstrates a subtle but potentially problematic issue related to CSS selector specificity.  The problem arises from the unexpected behavior of combining ID and class selectors within a single CSS rule. While developers generally understand the order of precedence between ID, class, and element selectors, the interaction of combined selectors can lead to unexpected results if not carefully considered.

## The Problem

The `bug.css` file shows a simple example where an ID selector (`#id-div`) and a class selector (`.special-div`) are both used to style the same element. While an ID selector usually takes precedence, the combination creates a more specific selector that overrides the individual selectors.

## The Solution

The `bugSolution.css` file demonstrates a possible way to avoid the issue. We can use a more organized approach, or if we are trying to avoid the `purple` color we need to make sure the `#id-div` selector is more specific.  Carefully understanding specificity is key to avoiding unexpected behavior in your CSS.