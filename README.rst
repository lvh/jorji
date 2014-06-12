=======
 jorji
=======

.. image:: https://travis-ci.org/lvh/jorji.svg
           :target: https://travis-ci.org/lvh/jorji

.. image:: https://coveralls.io/repos/lvh/jorji/badge.png
           :target: https://coveralls.io/r/lvh/jorji

This is Jorji:

.. image:: https://dl.dropboxusercontent.com/u/38476311/Logos/jorji.png
           :width: 200px

Jorji has a forged passp^H^H^H^H^Hcertificate:

.. image:: https://dl.dropboxusercontent.com/u/38476311/Logos/jorji-passport.png
           :width: 200px

Would you spot it? Would your software?

(Jorji and his passport are part of the excellent `Papers, Please`_, a
dystopian game about border control in a fictional communist country
by `Lucas Pope`_. Lucas has graciously allowed me to use the above
artwork, because he's awesome. You should go buy his games.)

``jorji`` (this project) contains the tools you need to produce a TLS
server (by default, an HTTPS server) with bogus certificates. This is
useful to write integration tests to verify that your application
actually checks the certificate provided by the server.

TLS clients have pretty much one job: verify certificates correctly.
Most clients don't bother to verify certificates at all, and give
forgeries way less credible than Jorji's passport a pass.

Using jorji
===========

Preparation
-----------

Create some bogus certs::

  >>> from jorji import make_cert
  >>> TODO

With Twisted
------------

If you're already using Twisted_::

  >>> from jorji import start
  >>> TODO

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

.. _`Papers, Please`: http://papersplea.se/
.. _`Lucas Pope`: http://dukope.com/
.. _Twisted: https://twistedmatrix.com/trac/
.. _crochet: https://github.com/itamarst/crochet
.. _Rackspace: http://www.rackspace.com/
.. _`lvh/jorji`: https://github.com/lvh/jorji
