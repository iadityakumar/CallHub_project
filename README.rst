CallHub Test
==============================

A Python/Django application that will display the Nth number in Fibonacci sequence. 
For instance, if N is 6 and the sequence starts with [1,1..] then it should display ‘8’ as the 6th element in the sequence.



Getting up and running
----------------------

The steps below will get you up and running with a local development environment. We assume you have the following installed:

* pip
* virtualenv

First make sure to create and activate a virtualenv_, then open a terminal at the project root and install the requirements for local development::

    $ pip install -r requirements.txt

.. _virtualenv: http://docs.python-guide.org/en/latest/dev/virtualenvs/

Run django migrations command for creating table::

    $ python manage.py makemigrations


    $ python manage.py migrate

You can now run the usual Django ``runserver`` command ::

    $ python callhubapp/manage.py runserver

For caching, its needed to setup redis-server and start the redis server on port 6379.

Testing
-------

For testing, you can use these commands::
    
    $ python manage.py test
    
For callhubapp test, you can use this::

    $ python manage.py test callhubapp
