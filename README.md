# Tailwind CSS @apply Directive Conflict

This repository demonstrates a bug where Tailwind CSS's `@apply` directive conflicts with custom directives when properties in the custom directive also exist in the base Tailwind CSS styles. This leads to unexpected style overrides.

## Bug Description
The `@apply` directive can unexpectedly override custom styles when there's a conflict with base Tailwind styles. This happens because the `@apply` directive's behavior might prioritize base styles over custom ones for conflicting properties.

## Reproduction
1. Clone this repository.
2. Examine the `bug.css` file.  Note the custom directive `my-custom-style` and how it is applied. 
3. Observe the unexpected visual output. 
4. Review the solution in `bugSolution.css` to see how to resolve this conflict.

## Solution
The solution involves careful naming or structuring of your custom directives to avoid naming collisions and ensure custom directives take precedence.