# CSS Specificity and Inheritance Conflict

This repository demonstrates a subtle bug related to CSS specificity and inheritance.  The `bug.css` file contains CSS code that unexpectedly fails to override inherited styles due to how specificity is handled in relation to inheritance. The `bugSolution.css` file provides a corrected version.

**Problem:**

In some cases, a CSS rule with higher specificity might not override an inherited style from a parent element.  This occurs when the specificity calculation happens *before* the inheritance resolution.  This is a less common issue, but can be confusing when debugging styles.