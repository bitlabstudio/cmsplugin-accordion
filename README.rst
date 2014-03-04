CMSPlugin Accordion
============

django-cms plugin that allow to create accordions on the frontend.

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    pip install cmsplugin-accordion

To get the latest commit from GitHub

.. code-block:: bash

    pip install -e git+git://github.com/bitmazk/cmsplugin-accordion.git#egg=cmsplugin_accordion

TODO: Describe further installation steps (edit / remove the examples below):

Add ``cmsplugin_accordion`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'cmsplugin_accordion',
    )

Add the ``cmsplugin_accordion`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^accordion/', include('cmsplugin_accordion.urls')),
    )

Before your tags/filters are available in your templates, load them by using

.. code-block:: html

	{% load cmsplugin_accordion_tags %}


Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate cmsplugin_accordion


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    mkvirtualenv -p python2.7 cmsplugin-accordion
    make develop

    git co -b feature_branch master
    # Implement your feature and tests
    git add . && git commit
    git push -u origin feature_branch
    # Send us a pull request for your feature branch
