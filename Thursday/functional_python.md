# Functional Python

**Speaker:** Paul Jones (@paulwilljones)
**Slides:** TODO
**Video:** TODO

- Main praradigms:
  - Imperative
  - Proceedural
  - Declarative
  - Logic
  - Functional

- Functional programming is:
  - No mutations, loops, or control structures; increases reusability.
  - Pure functions, first-class, higher functions.
  - Tail recursion.
  - Lazy evalution.

- Features:
  - Purity:
    - Functions with no side-effects.
    - No global state changes.
    - Same input == same output.
    
  TODO: too fast, update notes later ...
  
  - Partial functions, prepared arguments.
  
  - Immutability, leads to thread-safe code.
    - Python has some mutable types to help us here.
      - namedtuples
      - frozensets
      
  - Recursion, use tail recursion:
    - Python does not optimise this.
    - Trampolining can help here.
    
  - Lazy evalution:
    - In python use generators and iterators
    
  - In python map, reduce, and filter can be parallelised.
  
TODO: still too fast, update later.

- Use itertools, functools, operator, fn.py (Scala inspired), toolz, funcy

- Loot at Coconut (functional compiles to Python).
