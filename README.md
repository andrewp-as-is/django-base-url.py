<!--
https://readme42.com
-->


[![](https://img.shields.io/pypi/v/django-base-url.svg?maxAge=3600)](https://pypi.org/project/django-base-url/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/django-base-url.py/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/django-base-url.py/actions)

### Installation
```bash
$ [sudo] pip install django-base-url
```

#### How it works
settings `BASE_URL` if defined, else scheme+`request.get_host()`

##### `settings.py`
```python
TEMPLATE_CONTEXT_PROCESSORS = (
    "django_base_url.context_processors.base_url",
)
```

#### Examples
`settings.py`:
```python
BASE_URL="http://host/"
```

```html
<base href="{{ BASE_URL }}">
```

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>