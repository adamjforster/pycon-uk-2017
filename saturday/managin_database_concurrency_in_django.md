# Managing Database Concurrency in Django

**Speaker:** David Seddon (TODO)

**Slides:** TODO

**Video:** TODO


- Cuncurrent workers can cause issues with things like balances:
  - Worker 1 checks balance then removes funds
  - Worker 2 checks balance then removes funds
  - This can lead to double spending.
  
- Postgres's default isolation level is read commited.
  - Writes wait if another transaction is already writing (this uses a
    readonly lock).
  - `select_for_update()`delays read until readonly locks are released.
  
- Select for update on customer account (not ledger) can prevent double
  spending (pessimistic locking.)
