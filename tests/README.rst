=====
Tests
=====

This directory is a Django project, with ``testapp`` is an example app that
contains the tests and support code.

You can run the tests with the ``runtests.py`` script in the root of the repo.

You can also run Nexus locally to check changes in the browser with a simple
SQLite database with:

.. code-block:: bash

    ./manage.py runserver

This automatically adds the username 'admin' with password 'password' so you
can login locally at ``/admin/`` and peruse nexus at ``/nexus/``.

You can also manipulate ``PYTHONPATH`` to add other modules you might be
testing, e.g. if you have a ``gargoyle`` checkout in the same folder as
your ``nexus`` checkout, use:

.. code-block:: bash

    PYTHONPATH=../../gargoyle ./manage.py runserver

You'll need to change ``settings/base.py`` to add it there too, plus make sure
any dependencies are available as well.
