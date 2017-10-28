# Unsafe at Any Speed - Keynote

**Speaker:** Rae Knowler (@raeknowler)

**Slides:** https://speakerdeck.com/bellisk/unsafe-at-any-speed-pycon-uk-26th-october-2017

**Video:** TODO


- "The right thing to do is non-obvious, and the obvious thing to do is bad"

- Default aren't bad, bad defaults are bad.

- Bad defaults can cause:
  - Data loss
  - Security breaches
  - Becoming part of a bot net
  
- Examples:
  - CKAN default settings allowed public to create new organisations and upload
    new datasets.
  - MongoDB exposed 595.2 TB to the internet due to default open configuration
    with no auth requirement. Lots of data was wioed or ransomed. Fixed in 3.6
    but lots of people won't or can't upgrade.
  - Hadoop, Redis, and Elasticsearch (weird - TODO: get URL from slides).

- Sensible defaults could have prevented all of the above examples.

- "The 'S' in 'HTTPS' stands for secure" - PEP 476.
  - Before the PEP Python stdlib would not verify X509 certs.
  - People used requests instead.
  - Changes Aug 2014.

- Tom Eastman, 'Serialzation formats are not toys' talk.
  - PyYAML'd default is to use `load()` this will execute code.
  - Use `safe_load()` instead, prevent code injection.
  
- MongoDB pre-2.6 writes were fire and forget:
  - No error checking.
  - Writes failed silently.
  
- Why bad defaults are set:
  - Developer 'knows' the tool.
  - Unconsidered / changing use cases.
  - To make the tool feel 'easy'.
  - To make the tool performant.
  - Internal tools released externally.

- People don't do this on purpose (see quote from Li and Evans, Insecure by Default?).

- Zen of Python:
  - Explicit is better than implicit.
  - Errors should never pass silently.
  
- Good defaults:
  - Secure by default.
  - Reliable > performant.
  - Never silence errors.
  - Hard fail on serious errors.
  - If there is no safe default, ensure explicit configuration.
  - Be brave enough to fix bad defaults.
