---
template: overrides/main.html
title: Getting started
---

# Getting started

Material for MkDocs is a theme for [MkDocs][1], a static site generator geared
towards (technical) project documentation. If you're familiar with Python, you
can install Material for MkDocs with [`pip`][2], the Python package manager.
If not, we recommended using [`docker`][3].

In case you're running into problems, consult the [troubleshooting][4] section.

  [1]: https://www.mkdocs.org
  [2]: #with-pip
  [3]: #with-docker
  [4]: troubleshooting.md

## Installation

### with pip

Material for MkDocs can be installed with `pip`:

=== "Material for MkDocs"

    ```
    pip install mkdocs-material
    ```

=== "Material for MkDocs Insiders"

    ``` sh
    pip install git+https://${GH_TOKEN}@github.com/squidfunk/mkdocs-material-insiders.git
    ```

This will automatically install compatible versions of all dependencies:
[MkDocs][1], [Markdown][5], [Pygments][6] and [Python Markdown Extensions][7].
Material for MkDocs always strives to support the latest versions, so there's
no need to install those packages separately.

Note that in order to install [__Material for MkDocs Insiders__][8], you'll
need to [become a sponsor][9], create a [personal access token][10], and set
the `GH_TOKEN` environment variable to the token's value.

  [5]: https://python-markdown.github.io/
  [6]: https://pygments.org/
  [7]: https://facelessuser.github.io/pymdown-extensions/
  [8]: insiders.md
  [9]: insiders.md#how-to-become-a-sponsor
  [10]: https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token

### with docker

The official [Docker image][11] is a great way to get up and running in a few
minutes, as it comes with all dependencies pre-installed. Pull the image for the 
`latest` version with:

```
docker pull squidfunk/mkdocs-material
```

The `mkdocs` executable is provided as an entry point and `serve` is the 
default command. If you're not familiar with Docker don't worry, we have you
covered in the following sections.

The following plugins are bundled with the Docker image:

* [mkdocs-awesome-pages-plugin][12]
* [mkdocs-git-revision-date-localized-plugin][13]
* [mkdocs-minify-plugin][14]
* [mkdocs-redirects][15]

  [11]: https://hub.docker.com/r/squidfunk/mkdocs-material/
  [12]: https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin
  [13]: https://github.com/timvink/mkdocs-git-revision-date-localized-plugin
  [14]: https://github.com/byrnereese/mkdocs-minify-plugin
  [15]: https://github.com/datarobot/mkdocs-redirects

### with git

Material for MkDocs can be directly used from [GitHub][16] by cloning the
repository into a subfolder of your project root which might be useful if you
want to use the very latest version:

=== "Material for MkDocs"

    ```
    git clone https://github.com/squidfunk/mkdocs-material.git
    ```

=== "Material for MkDocs Insiders"

    ```
    git clone git@github.com:squidfunk/mkdocs-material-insiders.git mkdocs-material
    ```

The theme will reside in the folder `mkdocs-material/material`. Note that when
cloning from `git`, you must install all required dependencies yourself:

```
pip install -r mkdocs-material/requirements.txt
```

Note that in order to install [__Material for MkDocs Insiders__][8], you'll
need to [become a sponsor][9].

  [16]: https://github.com/squidfunk/mkdocs-material
