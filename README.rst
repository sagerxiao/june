June
=====

.. image:: https://travis-ci.org/pythoncn/june.png?branch=master
        :target: https://travis-ci.org/pythoncn/june
.. image:: https://coveralls.io/repos/pythoncn/june/badge.png?branch=master
        :target: https://coveralls.io/r/pythoncn/june

This is a forum project. Demo：http://python-china.org/

Installation
-------------

Make sure you have python2.7, pip and virtualenv installed.

Development
-----------

You should read the Contribution Guide first.

To start development server::

    $ git checkout your_fork_of_june
    $ cd june
    $ virtualenv --distribute venv
    $ source venv/bin/activate
    (venv)$ pip install -r requirements.txt
    (venv)$ alembic upgrade head
    (venv)$ python manager.py runserver

It should be running at localhost:5000.

Trouble shooting
----------------

If you encounter build failure when trying to install gevent and get error saying "event.h" not found. You need to install libevent before installing gevent again. 

On Mac OS X with homebrew, you can simply do::

    brew install libevent
