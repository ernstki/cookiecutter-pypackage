{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
{{ cookiecutter.project_name }}
{% for _ in cookiecutter.project_name %}={% endfor %}

{{ cookiecutter.project_short_description }}

{% if is_open_source %}
* Free software: {{ cookiecutter.open_source_license }}
* Documentation: <https://>{{ cookiecutter.project_slug | replace("_", "-") }}.readthedocs.io.
{% endif %}

Features
--------

-   TODO

Credits
-------

This package was created with
[Cookiecutter](https://github.com/audreyr/cookiecutter) and the
[ernstki/cookiecutter-pypackage](https://github.com/ernstki/cookiecutter-pypackage)
project template.
