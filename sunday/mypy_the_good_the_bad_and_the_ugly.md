# MyPy: The Good, The Bad and The Ugly

**Speaker:** David Sim (@Ramblin_Dave)

**Slides:** TODO

**Video:** TODO


- Static typing can:
  - Catch bugs early.
  - Increases code legibility.
  
- MyPy:
  - Option static type checker for python.
  - Used as a commandline tool.
  - Need to annotate your code with type hints.
  
- Challenges:
  - Some code is simply just dynamic (eval, pickle, JSON, Namedtuple).
    - Fixes:
      - Avoid this kind of code.
      - Use `isinstance()`.
      - Contain the dynamic stuff.
  -  Circular imports of type definitions (classes).
    - Fixes:
      - Wrap imports with `if False`, code won't be executed but MyPy will run
        as expected.
  - Missing libraries:
    - Fixes:
      - Create your own stubs.
      - Many stubs are bundled in MyPy.
  
- Good practises:
  - Use CI
  - Run in strict mode, explicitly exclude untyped code.
  
- Benefits:
  - Bugs were caught.
  - Brittle code was exposed.
  - Legibility was increased.

- Issues:
  - MyPy isn't mature yet.
  - Investment of time and training.
  
