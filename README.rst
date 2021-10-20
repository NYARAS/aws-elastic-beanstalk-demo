Deploying Simple Flask Application to AWS Elastic Beanstalk
===========================================================

Our Application
~~~~~~~~~~~~~~~

Our application is a simple "Hello World" example, and for the purpose of demostrating CI/CD using Github action
we have included s test case as well.

AWS Elastic Beanstalk
~~~~~~~~~~~~~~~~~~~~~

Our Flask application is going to be deployed to AWS Elastic Beanstalk which is a service that automates the deployement
and scalling of a web application. It takes your source code and takes care of all the infrustructure configuration.

How to install and run this project
-----------------------------------
Prerequisites
~~~~~~~~~~~~~
Make sure you have the following libraries installed before beginning:

- python3-dev
- redis-server
- git (`Configuring ssh`_)
- pip (`Installing pip`_)
- virtualenv & virtualenvwrapper `https://github.com/yyuu/pyenv <if using pyenv refer to this document>`_

Cloning from github
~~~~~~~~~~~~~~~~~~~
From your terminal go to the directory you want to clone the project into.

.. code:: bash

	$ cd path/to/your/directory

Clone the project.

.. code:: bash

	$ git clone git@github.com:NYARAS/aws-elastic-beanstalk-demo.git

Setting up the project's dependencies
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Navigate into the project directory from the terminal.

Setup the following dependencies.

 - `python-dev`_ 
 - `python3-dev`_ 

.. _python-dev: https://www.python.org/dev/
.. _python3-dev: https://www.python.org/dev/

.. code:: bash

	$ cd path/to/your/directory/aws-elastic-beanstalk-demo

Create a virtual environment to use for your project

.. code:: bash

  # Ignore this if you are not using virtualwrapper
  $ mkvirtualenv --python=/usr/bin/python3 env # env is the name of your virtual environment

From your virtualenv do the following.

.. code:: bash

	(env)$ pip install -r requirements.txt # run this in a clean virtualenv

.. _Configuring ssh: https://help.github.com/articles/generating-ssh-keys/
.. _Installing pip: https://pip.pypa.io/en/stable/installing/#installing-with-get-pip-py