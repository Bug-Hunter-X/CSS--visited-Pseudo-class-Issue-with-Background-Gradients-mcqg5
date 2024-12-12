# CSS :visited Pseudo-class Issue with Background Gradients

This repository demonstrates a subtle issue with the CSS `:visited` pseudo-class when used with `background-image` and linear gradients.  The expected behavior is that the background image should change upon visiting a link. However, in some browsers, only the initial change is observed; subsequent visits do not trigger the style update.

## Bug Description:
The provided CSS applies a linear gradient as a background. The `:visited` pseudo-class attempts to alter the gradient on subsequent visits.  However, this often fails to update properly due to specificity conflicts or browser rendering quirks.

## Solution:
The solution provides an approach to ensure proper style updates using the `!important` flag to override the default style.

## How to reproduce:
1. Create an HTML file (e.g., `index.html`).
2. Link the `bug.css` stylesheet to the HTML.
3. Create a link tag in the HTML.
4. Observe that the background-image does not update properly.
5. Replace `bug.css` with `bugSolution.css` and observe the fix.
