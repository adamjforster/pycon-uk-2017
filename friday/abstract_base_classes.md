# Abstract base Classes

**Speaker:** Leonardo Giordani ([@thedigicat](https://twitter.com/thedigicat))

**Slides:** TODO

**Video:** TODO


- In python it is EAFP.
  - We test for behaviour not structure (duck typing).
  - How do we test that something behaves in a complex way? For instance like a
    list? This is hard.
  - It's tempting to fallback to `isinstance` to just check the type.
  - Type checking doesn't work when we're interessted in behaviours.
  - In a perfect world we'd have a `behaveslike` function, but we don't.
  
- Python is based on delegation (inheritance and composition).
  - Python now has `__isinstancecheck__` methods, so can treat `isinstance` like
    `behaveslike` with a behaviour class.
    
- Classes that register subclasess are calles ABCs.
  - `Sequence.register(tuple)`
  - This is a promise, not a check.
  
- Abstract Base Classes are categories (labels).

- Read the docs on ABCs.

- MetaClasses:
  - When you build an instance you use a class.
  - When you build a class you can use metaclass.
  - Don't be scared of metaclasses.
  - metaclasses are inherited.
  - metaclasses > decorators because they have inheritance.
