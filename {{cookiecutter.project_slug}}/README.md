[![Docker Stars](https://img.shields.io/docker/stars/{{ cookiecutter.username }}/{{ cookiecutter.project_slug }}.svg?style=flat-square)](https://hub.docker.com/r/{{ cookiecutter.username }}/{{ cookiecutter.project_slug }}/)
[![Docker Pulls](https://img.shields.io/docker/pulls/{{ cookiecutter.username }}/{{ cookiecutter.project_slug }}.svg?style=flat-square)](https://hub.docker.com/r/{{ cookiecutter.username }}/{{ cookiecutter.project_slug }}/)

{{ cookiecutter.project_short_description }} Docker image
{{ '=' * cookiecutter.project_name | length }}{{ '=' * (' Docker image' | length) }}

{{ cookiecutter.description }}

Download size of this image is only:
[![](https://images.microbadger.com/badges/image/{{ cookiecutter.username }}/{{ cookiecutter.project_slug }}.svg)](http://microbadger.com/images/{{ cookiecutter.username }}/{{ cookiecutter.project_slug }} "Get your own image badge on microbadger.com")


Docker Hub Build
----------------

This template assumes you to be registered in Docker Hub.
To setup automated build via Docker Hub refer to: [Set up Automated builds](https://docs.docker.com/docker-hub/builds/).

To configure automated builds follow this link [Build configurations](https://cloud.docker.com/u/{{ cookiecutter.username }}/repository/docker/{{ cookiecutter.username }}/{{ cookiecutter.project_slug }}/builds/edit)


Usage Example
-------------

This image is intended to be a base image for your projects, so you may use it like this:

```
Dockerfile
    FROM {{ cookiecutter.username }}/{{ cookiecutter.project_slug }}

    COPY ./my_app /usr/local/bin/my_app
```

```
sh
    $ docker build -t my_app .
```

License
-------

This project is licensed under: [{{ cookiecutter.open_source_license }}]({%- if cookiecutter.open_source_license == 'MIT' -%}
https://tldrlegal.com/license/mit-license
{%- elif cookiecutter.open_source_license == 'BSD-2-Clause' -%}
https://tldrlegal.com/license/bsd-2-clause-license-(freebsd)
{%- elif cookiecutter.open_source_license == 'BSD-3-Clause' -%}
https://tldrlegal.com/license/bsd-3-clause-license-(revised)
{%- elif cookiecutter.open_source_license == 'Apache-2.0' -%}
https://tldrlegal.com/license/apache-license-2.0-(apache-2.0)
{%- elif cookiecutter.open_source_license == 'GPL-2.0-only' -%}
https://tldrlegal.com/license/gnu-general-public-license-v2
{%- elif cookiecutter.open_source_license == 'GPL-3.0-only' -%}
https://tldrlegal.com/license/gnu-general-public-license-v3-(gpl-3)
{%- elif cookiecutter.open_source_license == 'LGPL-2.1-only' -%}
https://tldrlegal.com/license/gnu-lesser-general-public-license-v2.1-(lgpl-2.1)
{%- elif cookiecutter.open_source_license == 'LGPL-3.0-only' -%}
https://tldrlegal.com/license/gnu-lesser-general-public-license-v3-(lgpl-3)
{%- elif cookiecutter.open_source_license == 'Not licensed' -%}
https://choosealicense.com/no-permission/
{% endif %})


Attributions
------------

Add below authors and licenses from which your work derives from, if any.

This work is derived from the work of:

| Author            | Work Source                                  | License                      |
|:------------------|:---------------------------------------------|:-----------------------------|
| Add Some Author   | <https://some-author-work-source-url>        | [some-author-license.txt](./attributions/some-author-license.txt) |

References
----------

List of references
