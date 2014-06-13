=======================
 Contributing to jorji
=======================

Thank you for your interest in contributing to jorji!

Please send pull requests to `lvh/jorji`_ on Github. All changes go
through peer review before merging. All changes must come with full
test coverage to be merged. (If it's unclear how to test something,
it's always okay to send in pull requests for review.)

jorji uses tox_ for automated testing. Install it and run it in the
root directory of the repository, and it will automatically build
virtualenvs for all of the supported Python interpreters, with all of
the dependencies installed. It will run the test suite, which includes
unit tests as well as various style guide tests.

Among other things, jorji complies with the recommendations set forth
in PEP8_ and PEP257_. Consult the output of tox for full details on
any potential style issues.

If you found some ``-----BEGIN RSA PRIVATE KEY-----`` lines in the
repository by automated search, that is not a bug.

.. _`tox`: http://tox.readthedocs.org/en/latest/
.. _`lvh/jorji`: https://github.com/lvh/jorji
