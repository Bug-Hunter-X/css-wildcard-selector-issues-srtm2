# Unexpected CSS Styling Due to Overly Broad Wildcard Selector

This repository demonstrates a subtle bug in CSS involving the use of a wildcard selector in combination with the child combinator.  The issue arises from the unintended consequences of applying a style to *all* direct children of a parent element.

## Bug Description
The `bug.css` file contains a CSS rule that uses the selector `.container > *`. While seemingly straightforward, this selector applies styles to all direct children of elements with the class `container`. If you add elements inside `.container` that were not intended to have these styles, it leads to unexpected visual results.

## Solution
The `solution.css` file offers a solution to this problem.  Rather than using the wildcard, it uses more specific selectors to target only the intended elements within the `.container`.

This demonstrates the importance of writing precise CSS selectors to avoid unexpected behavior and maintain better control over styling.