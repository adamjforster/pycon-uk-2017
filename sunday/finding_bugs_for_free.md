# Findinh Bugs for Free: the Magic of Code Analysis

**Speaker:** Mark Shannon (TODO)

**Slides:** TODO

**Video:** https://www.youtube.com/watch?v=lAvTq4PhM4M


- Static code analysis, learning aout your code without executing it.
  - Automated code review.
  
- Good code analysis is:
  - Flexible, extensible.
  - Accurate, don't waste user time with false positives.
  - Insightful, finds non-trivial bugs.

- We can do this for python but it's harder than statically typed languages.

- What makes lgtm flexible?
  - OO modular query language.
  - Simple queries.

- What makes lgtm accurate?
  - Abstract syntax tree to check syntax issues.
  - Control flow graph to check execution flow issues.
  - Call context to check flow based on parameters.

- 
