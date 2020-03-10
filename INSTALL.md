---
layout: page
title: Installation
permalink: /install
---

`wtss.py` depends essentially on
[Requests](https://requests.readthedocs.io/en/master/). Please, read the
instructions below in order to install `wtss.py`.

## Production installation


**Under Development!**

## Development installation

Clone the software repository:

~~~shell
$ git clone https://github.com/brazil-data-cube/wtss.py.git
~~~

Go to the source code folder:

~~~shell
$ cd wtss.py
~~~

Install in development mode:

~~~shell
$ pip3 install -e .[all]
~~~

Run the tests:

~~~shell
$ ./run-test.sh
~~~

Generate the documentation:

~~~shell
$ python setup.py build_sphinx
~~~

The above command will generate the documentation in HTML and it will
place it under:

~~~shell
doc/sphinx/_build/html/
~~~
