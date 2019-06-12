# hackoregon_sample_django

![PyPI version](https://badge.fury.io/py/2019-sample-django-backend.svg) | [![Build Status](https://travis-ci.org/hackoregon/2019-sample-django-backend.svg?branch=master)](https://travis-ci.org/hackoregon/2019-sample-django-backend)

This is just a project to show what a default cookiecutter for Civic Cookiecutter Django looks like when run.

# Documentation

The full documentation is at http://hackoregon.github.io/2019-sample-django-backend


# Features

> -   TODO (add what your project does)

# Data Sources

This API package in this repo is based on the Data Science work in the following projects:

* [Name of repo where data science work is contained](URL of repo where data science work is contained)

# Quickstart to install package in your own Django Project (Non-Hack Oregon Workflow)

* Install hackoregon_sample_django:  
  `pip install hackoregon_sample_django`

* Add subpackages to your `INSTALLED_APPS`:

  ```python
  INSTALLED_APPS = [     
                      ...     
                      'sampler',     
                      ...
                    ]
  ```

* Add hackoregon_sample_django's URL patterns:

  ```python
  from hackoregon_sample_django.sampler
  import urls as sampler_urls   

  urlpatterns = [     
                  ...     
                  url(r'^', include(sampler_urls)),     
                  ...
                ]
  ```

* Setup your database with a matching schema

* Run the project

# Running Tests

This repo uses pytest and pytest-django to run tests.

For project development work, tests will be run in docker container
using the bin/test.sh script:

# Credits

Tools used in rendering this package:

 * [Cookiecutter](https://github.com/audreyr/cookiecutter)
 * [cookiecutter-djangopackage](https://github.com/pydanny/cookiecutter-djangopackage)
