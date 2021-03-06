gethy
------
GET Hy the Fastest Way!

Installation
============

For Direct Use
~~~~~~~~~~~~~~

Because it's at early stage, installing from GitHub is the preferred way.

.. code:: bash

  $ pip install git+https://github.com/CreatCodeBuild/gethy

You can also install it from PyPi. But the version could be behind GitHub's master branch.

.. code:: bash

  $ pip install gethy

For Development
~~~~~~~~~~~~~~~

.. code:: bash

  $ git clone https://github.com/CreatCodeBuild/gethy
  $ cd gethy
  $ pip install . -e .[test]
  
Supported Version
=================
- CPython3.5
- CPython3.6
- PyPy3.5 v5.9
Other versions and implementations of python should work. (Not tested)

No Python3 specific syntax or technique used. But, hey, this is 2017! Python3 came out 8 years ago and Obama was out of office. Just deal with it.

GetHy?
======
GetHy is pronounced "Get high". It stands for "Get Hypertext Transfer Protocol". It is one of those awkward word-playing jokes.

GetHy is an application level IO indenpent HTTP/2 library. It can be used in any IO model and is super easy to use.

HTTP was intended to be a stateless protocol. At my best understanding, 
HTTP/2 changes that a little bit at the Session and Presentation level.

Therefore, using HTTP/2 directly is a little bit counter intuitive if you are used to the stateless Request-Response model. 
However, HTTP/2 at an Application level is or should be still stateless. It doesn't change the HTTP semantics for application/Web developers.

This library utilizes the powerful and only Python HTTP/2 library `h2 <https://github.com/python-hyper/hyper-h2>`_.

h2 is not an application level library in terms of that it doesn't provide the GET, POST kind of semantics for the user. 
GetHy builds on top of h2 and provides the user Web level semantics.

Like h2, GetHy does not do IO at all! You are free to use whatever IO model.

Off course you should use coroutines. Because you should check out my Web framework `hyper2web <https://github.com/CreatCodeBuild/hyper2web>`_.


Contribution
============
All contributions are welcome. You can simply submit a pull request. Please clearly descript your PR in comments.

You can also use Issues to start a discussion or question.
