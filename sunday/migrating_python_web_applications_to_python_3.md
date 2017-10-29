# Migrating Python Web Applications to Python 3

**Speaker:** Andrew Wray (TODO)

**Slides:** https://w0rp.com/presentation/migrating

**Video:** TODO


- Why python 3?
  - Bug fixes.
  - Better types.
  - Django 2.
  - Less memory consumption in production (lazy sequences?)
  - Python 2.7 will only be maintined for security.
  
- Upgrade process (important see slides!)
  - Installing python 3:
    - Use dead snakes repo on Ubuntu.
  - Use CI to test against both 2 and 3.
  - Use different virtualenvs for local.
  - Update all files to use `__future__` imports to enable python 3!
  - Install si for a compatability layer.
  
- Issues:
  - Builtins, `xrange` in now `range`, `range` is not `list(range)`.
  - Use list comps instead of `map` and `filter`
  -`reduce` removed in python 3.
  - type checking (use six).
  - text and bytes, use `__future__` import.
  
