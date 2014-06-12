=======
 jorji
=======

.. image:: https://travis-ci.org/lvh/jorji.svg
           :target: https://travis-ci.org/lvh/jorji

.. image:: https://coveralls.io/repos/lvh/jorji/badge.png
           :target: https://coveralls.io/r/lvh/jorji

jorji has a forged passp^H^H^H^H^Hcertificate. Will you catch it?

This contains the tools you need to produce a TLS server (by default,
an HTTPS server) with bogus certificates. This is useful to write
integration tests to verify that your application actually checks the
certificate provided by the server.

Using jorji
===========

With Twisted_
------------

If you're already using Twisted,

```python
from jorji import make_cert, run
TODO!!!
```

Without Twisted (a.k.a. with Twisted, secretly, anyway)
-------------------------------------------------------

The recommended way to use jorji without Twisted is crochet_. It will
run the Twisted reactor off in a thread somewhere so you don't have to
worry about it.

Thanks!
=======

I'd like to thank Rackspace_ for giving me the opportunity to produce
open-source software on company time.

Contributing to jorji
=====================

Please send pull requests to `lvh/jorji`_ on Github.

.. _Twisted: https://twistedmatrix.com/trac/
.. _crochet: https://github.com/itamarst/crochet
.. _Rackspace: http://www.rackspace.com/
.. _`lvh/jorji`: https://github.com/lvh/jorji
