celery-statsd
=============
Fork of [celery-statsd](https://github.com/ssaw/celery-statsd) to work with [datadog](https://www.datadoghq.com/).


In your `tasks.py`

```python
import celery_statsd
```

And in your settings file set `STATSD_HOST` and `STATSD_PORT`.

You will now have stats about your tasks in statsd.

By default stats will be published with a key prefix of "celery.". Change the CELERYD_STATS_PREFIX
if you want something different.
