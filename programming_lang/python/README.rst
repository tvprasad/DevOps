Gatsby Python Wiki
==================

Path
----

.. code-block:: python

  python -c "import sys; print('\n'.join(sys.path))"


Install mysqlclient-python
----

.. code-block:: bash

  LDFLAGS=-L/usr/local/opt/openssl/lib pip install mysqlclient

Python 2.7 Console printing issue
---------------------------------

.. code-block:: python

    import sys
    import codecs
    codecs.register(lambda name: codecs.lookup('utf-8') if name == 'cp65001' else None)
    if sys.stdout.encoding != 'UTF-8':
        sys.stdout = codecs.getwriter('utf-8')(sys.stdout, 'strict')
    if sys.stderr.encoding != 'UTF-8':
        sys.stderr = codecs.getwriter('utf-8')(sys.stderr, 'strict')


Strip
-----

* https://stackoverflow.com/questions/38285654/why-is-str-strip-so-much-faster-than-str-strip


External References
-------------------
* https://docs.python.org/3/
* https://www.python.org/dev/peps/pep-0440/
* https://pypi.org/project/
* https://test.pypi.org/
* https://github.com/dgrunwald/rust-cpython
* https://github.com/python/cpython
* https://github.com/crazyguitar/pysheeet
* How to get string objects instead of Unicode from JSON?: https://stackoverflow.com/questions/956867/how-to-get-string-objects-instead-of-unicode-from-json?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa

Korean Doc: https://docs.python.org/ko/3/

https://awesome-python.com/
