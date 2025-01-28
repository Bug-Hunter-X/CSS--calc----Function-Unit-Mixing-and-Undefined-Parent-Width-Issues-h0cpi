# CSS `calc()` Function: Unit Mixing and Undefined Parent Width Issues

This repository demonstrates a potential issue with the CSS `calc()` function involving unit mixing and situations where the parent element's width is not explicitly defined.  The `bug.css` file contains the problematic code, while `bugSolution.css` offers potential solutions.

The core problem is that while `calc(50% - 10px)` is generally well-supported, unexpected results might occur if:

1. **Unit Mixing Inconsistencies:** Certain browsers might have issues if the unit mix within `calc()` is not entirely consistent.
2. **Undefined Parent Width:** If the parent element's width is not explicitly defined or is determined dynamically, the calculation within `calc()` can become unreliable and may produce unexpected results or layout issues.

The solutions in `bugSolution.css` address these problems.