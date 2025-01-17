# CSS Specificity Bug

This repository demonstrates a common yet subtle issue in CSS: unexpected style overriding due to selector specificity.  The problem arises when selectors with varying specificity conflict, leading to unexpected visual results.

The `bug.css` file contains the erroneous code, while `bugSolution.css` presents a corrected approach.

## Understanding Specificity

CSS specificity determines which style rule takes precedence when multiple rules apply to the same element. More specific selectors override less specific ones.  The provided example highlights this concept, where a more specific selector unintentionally overwrites a general style rule.

## How to Reproduce

1. Open `bug.css`.
2. Observe that despite setting the `p` selector to blue, the text within the `div` appears red.
3. Open `bugSolution.css` to see a resolved version.

## Solution

The solution lies in understanding and managing specificity.  If you want to ensure consistent styling, you should review your selectors carefully, prioritizing the use of more specific styles when required, and carefully handle cascading styles and their priorities.