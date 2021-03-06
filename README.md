![](http://media.charlesleifer.com/blog/photos/scout.png)

[scout](http://scout.readthedocs.org/en/latest/) is a RESTful search server written in Python. The search is powered by [SQLite's full-text search extension](http://sqlite.org/fts3.html), and the web application utilizes the [Flask](http://flask.pocoo.org) framework.

Features:

* Multiple search indexes present in a single database.
* RESTful design for easy indexing and searching.
* Simple key-based authentication (optional).
* Lightweight, low resource utilization, minimal setup required.
* Store search content and arbitrary metadata.
* Multiple result ranking algorithms, porter stemmer.
* Comprehensive unit-tests.
* [Documentation hosted on ReadTheDocs](http://scout.readthedocs.org/en/latest/).

## Installation

Scout can be installed from PyPI using `pip` or from source using `git`. Should you install from PyPI you will run the latest version, whereas installing from `git` ensures you have the latest changes.

Installation using pip:

```console
$ pip install scout
```

You can also install the latest `master` branch using pip:

```console
$ pip install -e git+https://github.com/coleifer/scout.git#egg=scout
```

If you wish to install from source, first clone the code and run `setup.py install`:

```console
$ git clone https://github.com/coleifer/scout.git
$ cd scout/
$ python setup.py install
```

Using either of the above methods will also ensure the project's Python dependencies are installed: [flask](http://flask.pocoo.org) and [peewee](http://docs.peewee-orm.com).

[Check out the documentation](http://scout.readthedocs.org/en/latest/) for more information about the project.
