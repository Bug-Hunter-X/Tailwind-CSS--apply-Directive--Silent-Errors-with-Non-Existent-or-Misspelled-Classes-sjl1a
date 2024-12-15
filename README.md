# Tailwind CSS @apply Directive: Silent Errors with Non-Existent or Misspelled Classes
This repository demonstrates a subtle bug in Tailwind CSS related to the `@apply` directive. When using `@apply` with an invalid class name, Tailwind might not always generate an error, leading to unexpected styling issues.

## Problem
The `@apply` directive is incredibly convenient for reusing styles, however if you mistype a class or attempt to apply a class that does not exist, you might not get an error and end up with unexpected results in your CSS output.

## Solution
The best way to avoid this is to make sure the spelling of the classes you use with `@apply` is accurate and that these classes are actually defined in your Tailwind configuration.  Using a linter and/or a Tailwind CSS IntelliSense extension for your code editor can also help significantly.