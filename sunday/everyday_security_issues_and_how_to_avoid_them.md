# Everyday Security Issues and How to Avoid Them

**Speaker:** Chrisitan Heimes (@ChristianHeimes)

**Slides:** TODO

**Video:** TODO


- Security breachs can result in the loss of huge sums of money, or even the
  loss of life.
  
- Why is security hard?
  - Systems are complex.
  - Weak links cause catastrophic failure.
  - Security is not testable.
  - Built-in design issues.
  - Threat analysis is difficult.
  
- Lot's of good points, see slides.

- Python dangerous features:
  - `exec()`
  - `eval()`
  - `import`, `__import__`
  - `pickle`, `marshal`
  - `ctypes`
  
- More good stuff, see slides.

- Don't use XML!!!

- Don't implement your own crypto.

- UsE `os.urandom()`not `random.random()`.
