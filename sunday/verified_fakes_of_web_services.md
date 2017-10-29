# Verified fakes of Web Services

**Speaker:** Adam Dangoor (@adamdangoor)

**Slides:** TODO

**Video:** TODO


- Testing against a live API causes problems:
  - Slow.
  - Costly.
  - ...
  
- Can we test that our code is calling the API correctly, even when the API is
  down?
  - Yes, with mocks.
  
- `pip install requests-mock`

- pytest's fixture context managers are useful here.

- Problems with mocking:
  - Human error.
  - API changes lead to outdated mocks.
  
- Writing a mock:
  - A verified fake is a mock that can pass a  test suite that can be run
    against either a real API.
  - Parameterising tests (see slides for details).
  - The tests now tell us when the API has breaking changes.
    - Use a scheduled test suite to test this periodically.
    
- Shipping a verified fake will add value to your software.
