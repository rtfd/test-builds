environment-variables
=====================

These are the environment variables used to build this docs:

.. runblock:: pycon

   >>> import os
   >>> import pprint
   >>> pprint.pprint(dict(os.environ))

There is a variable called ``SECRET_VALUE_ESCAPED`` with this content
``{1}\|\1+-(8)$`` that should be shown correctly.

----

Sphinx configuration file used to build this docs (:doc:`see full file <conf>`),

.. literalinclude:: conf.py
   :language: python
   :end-before: ###########################################################################
   :linenos:

----

.. runblock:: pycon

   >>> # Build at
   >>> import datetime
   >>> datetime.datetime.utcnow()  # UTC
