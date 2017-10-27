# Single Malt WSGI

**Speaker:** Simon Davy (@bloodearnest)

**Slides:** TODO

**Video:** TODO


- WSGI is the standard in the python community.

- Our services are kbeautiful snow flakes, but wish they were cheap cool sheep.

- Warning: the following are strongly held opinions:
  - Tools need to be both useful and usable.
  - Be conservative in what you send.
  - Use production safe defaults. 

- Talisker is designed to integrate all the things!
  - A single point of control:
    - Tested.
    - Released.
    - Versioned.
    - Documented.
    - Audited.

- Talisker provides:
  - talisker.gunicorn
  - talisker.celery
  - talisker.run (great for cronjobs)

- Metrics:
  - To statsd / prometheus.
  - RED (rate, errors, duration).
  - HTTP req / res.
  - Celery tasks.
  - Scripts (cron).

- Standardised urls: ping, check, metrics, etc ...

- Error reporting: WSGI, Django, Celery, scripts, etc ...
  - Uses Sentry breadcrumbs
  
- Tracing: add request IDs to all the things.

- Logging:
  - Uses stdlib logging.
  - Log to stderr (usable everywhere), avoids python stdout buffering.
  - Uses logfmt.
  - Sent to logstash.
