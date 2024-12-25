# CSS calc() Unexpected Behavior with Mixed Units

This repository demonstrates a common issue encountered when using the `calc()` function in CSS with a mixture of percentage and other units (like `em` or `rem`).  The problem stems from the different reference points for these units:

* **Percentages (%)**: Relative to the containing element's width.
* **ems (em)**: Relative to the parent element's font size.
* **rems (rem)**: Relative to the root element's font size.

This difference in context can lead to unexpected layout results. The example illustrates the issue and provides a solution.

## Files:

* `bug.css`: Demonstrates the problematic CSS code.
* `bugSolution.css`: Shows how to avoid this problem.

## How to reproduce:

1. Clone this repository.
2. Open `index.html` (you'll need to create a simple HTML file to test this) in your browser.
3. Observe the unexpected layout due to the `calc()` function in `bug.css`.
4. Replace `bug.css` with `bugSolution.css` and observe the corrected layout.