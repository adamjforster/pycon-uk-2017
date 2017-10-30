# Python as a Second Language

**Speaker:** Hannah Hazi

**Slides:** TODO

**Video:** TODO


- Programmers suffer from 'baby duck syndrome'.
- Every language has it's own version of good style.

- Why bother to become fluent?
  - It makes life easier.
  - It makes code reviews better.
  - It reduces bugs.

- From OO background?
  - See 'Stop Writing Classes' by Jack Diederich.
    - There are easier ways to do things in Python than using classes.
  - Don't use getters and setters, use attributes and @property.

- From low level?
  - (Over)use global keyword.
  - Over-complicate loops (comprehensions ftw!)
  - Pixel shortage, use longer descriptive variable names.
  - Longing for static types, don't name variables with types.

- Python developers should be responsible adults.
  - Just because it's possible doesn't mean it's a good idea.
  
- Protected and private variables are just conventions, avoid private (__).

- The most diabolical anti-pattern: passing all exceptions silently!
  - Catch the exception that you expect and log it appropriately.

- Lookup the Anti-Zen of Python by Daniel Greenfeld.
