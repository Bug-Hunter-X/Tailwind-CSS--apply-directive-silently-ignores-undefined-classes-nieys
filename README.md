# Tailwind CSS @apply Silent Failure

This repository demonstrates a subtle issue with Tailwind CSS's `@apply` directive. When you use `@apply` with a class that doesn't exist or has a typo, Tailwind doesn't throw an error. Instead, it simply ignores the directive, leaving you scratching your head when your styles don't appear.

This can be very difficult to debug, especially in larger projects.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` to install Tailwind CSS (if necessary).
3. Open `bug.html` in your browser.  You'll notice that the paragraph text doesn't have the expected green color because `non-existent-class` is not defined.
4. View `bugSolution.html` for a solution implementing class existence check