# PostgreSQL: Beyond the Basics

**Speaker:** Lorna Mitchell (@lornajane)

**Slides:** TODO

**Video:** TODO

- Postgres has awesome data types:
  - UUID, great to use as a primary key, probably no collisions.
    - Great with `returning` keyword:
        - Return a value from a row after an insert or update.
  - JSON/JSONB, use JSONB it allows direct access / filtering of JSON data 😃
  
- Indexes:
  - Everything should have a primary key.
    - Serial for incremented ints.
  - Unique keys.
  - Lookup columns (groups of columns, composite keys).
  - Indexes can be created with expressions (eg the lowercase version of the name column).
  
- SQL:
  - Joining tables to themselves, great for building trees.
  - Aggregate functions
    - `GROUP BY` is the magic sauce.
    - `HAVING` is a `WHERE` for aggregates.
  - Common table expressions (CTE).
    - For making resuable composite tables.
    - Define with `WITH` and then use with a `JOIN`.
  - Window functions.
    - Allow us to calculate aggregate values whilst still returning the individual rows!
