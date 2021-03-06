[![Docker Stars](https://img.shields.io/docker/stars/{{ cookiecutter.username }}/{{ cookiecutter.docker_image_name }}.svg?style=flat-square)](https://hub.docker.com/r/{{ cookiecutter.username }}/{{ cookiecutter.docker_image_name }}/)
[![Docker Pulls](https://img.shields.io/docker/pulls/{{ cookiecutter.username }}/{{ cookiecutter.docker_image_name }}.svg?style=flat-square)](https://hub.docker.com/r/{{ cookiecutter.username }}/{{ cookiecutter.docker_image_name }}/)

{{ cookiecutter.project_short_description }} Docker image
{{ '=' * cookiecutter.project_name | length }}{{ '=' * (' Docker image' | length) }}

{{ cookiecutter.description }}

Download size of this image is only:
[![](https://images.microbadger.com/badges/image/{{ cookiecutter.username }}/{{ cookiecutter.docker_image_name }}.svg)](http://microbadger.com/images/{{ cookiecutter.username }}/{{ cookiecutter.docker_image_name }} "Get your own image badge on microbadger.com")


Usage Example
-------------

This image is intended to be a base image for your projects, so you may use it like this:

```
Dockerfile
    FROM {{ cookiecutter.username }}/{{ cookiecutter.docker_image_name }}

    COPY ./my_app /usr/local/bin/my_app
```

```
sh
  $ docker build -t my_app .
```

Build image in Docker Hub 
-------------------------

This template assumes you to be registered in Docker Hub.
To setup automated build via Docker Hub refer to: [Set up Automated builds](https://docs.docker.com/docker-hub/builds/).

To configure automated builds follow this link [Build configurations](https://cloud.docker.com/u/{{ cookiecutter.username }}/repository/docker/{{ cookiecutter.username }}/{{ cookiecutter.docker_image_name }}/builds/edit)


Release a new image
-------------------

Make your changes and bump the image version with one of the commands, depending on the version bump:

```
sh
  $ bump2version part major
  $ bump2version part minor
  $ bump2version part patch
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
