# Lazy Sequences Working Hard

**Speaker:** Thomas Guest (@thomasguest)

**Slides:** TODO

**Video:** TODO


- Lazy sequences yield values when they are needed.
  - This makes it possible to work with large datasets with limited resources.
  - They can be chained together.
  - Python is good at this. 

- `range()` creates a range object, not a collection in memory.
  - In python 2 use `xrange()`.
  
- `map()`, `filter()`, and `dict.keys()` are all now lazy in python 3.

- Generator offer language level access to lazy sequences
  - They use the `yield` statement.
  - You can't go backwards or call `len()`.

- Generator expressions, work like comprehensions but for generators.

- itertools module is useful for working with lazy sequences.
  - It has `groub_by()`!
