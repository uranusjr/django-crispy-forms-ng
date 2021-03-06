=======================
django-crispy-forms-ng
=======================

.. image:: https://travis-ci.org/uranusjr/django-crispy-forms-ng.svg?branch=ng
   :alt: Build Status
   :target: https://travis-ci.org/uranusjr/django-crispy-forms-ng

django-crispy-forms-ng is a fork of `django-crispy-forms`_. The original project, lead by `Miguel Araujo`_, stopped receiving update during early 2014. The problem grew with each Django upgrade, and more and more functionalities relied by it became deprecated.

This fork aims to provide support to modern Django versions, while maintain reasonable support for older versions. The plan is to support all officially supported major Django versions, and all versions between the oldest LTS version to the current version. For example, as of April 2015, the latest Django version is 1.8, while the oldest LTS version is 1.4, so the supported Django versions are 1.4–1.8.

The original django-crispy-forms README follows.


.. _`django-crispy-forms`: https://github.com/maraujop/django-crispy-forms

------


The best way to have Django_ DRY forms. Build programmatically reusable layouts out of components, having full control of the rendered HTML without writing HTML in templates. All this without breaking the standard way of doing things in Django, so it plays nice with any other form application.

The application mainly provides:

* A filter named ``|crispy`` that will render elegant div based forms. Think of it as the built-in methods: ``as_table``, ``as_ul`` and ``as_p``. You cannot tune up the output, but it is easy to start using it.
* A tag named ``{% crispy %}`` that will render a form based on your configuration and specific layout setup. This gives you amazing power without much hassle, helping you save tons of time.

Django-crispy-forms supports several frontend frameworks, such as Twitter `Bootstrap`_ (versions 2 and 3), `Uni-form`_ and Foundation. You can also easily adapt your custom company's one, creating your own, `see the docs`_ for more information. You can easily switch among them using ``CRISPY_TEMPLATE_PACK`` setting variable.

.. _`Uni-form`: http://sprawsm.com/uni-form
.. _`Bootstrap`: http://twitter.github.com/bootstrap/index.html
.. _`see the docs`: http://django-crispy-forms.rtfd.org

Authors
=======

django-crispy-forms is the new django-uni-form. django-uni-form was an application created by `Daniel Greenfeld`_ that I leaded since version 0.8.0. The name change tries to better explain the purpose of the application, which changed in a significant way since its birth.

If you are upgrading from django-uni-form, we have `instructions`_ for helping you.

* Lead developer: `Miguel Araujo`_

.. _`Daniel Greenfeld`: https://github.com/pydanny
.. _`Miguel Araujo`: https://github.com/maraujop
.. _`instructions`: http://django-crispy-forms.readthedocs.org/en/1.1.1/migration.html

Example
=======

This is a teaser of what you can do with latest django-crispy-forms. `Find here the gist`_ for generating this form:

.. image:: http://i.imgur.com/LSREg.png

.. _`Find here the gist`: https://gist.github.com/1838193

Documentation
=============

For extensive documentation see the ``docs`` folder or `read it on readthedocs`_

.. _`read it on readthedocs`: http://django-crispy-forms.readthedocs.org/en/latest/index.html

Special thanks
==============

* To Daniel Greenfeld (`@pydanny`_) for his support, time and the opportunity given to me to do this.
* The name of the project was suggested by the fantastic Audrey Roy (`@audreyr`_)
* To Kenneth Love (`@kennethlove`_) for creating django-uni-form-contrib from which bootstrap template pack was started.

.. _`@audreyr`: https://github.com/audreyr
.. _`@pydanny`: https://github.com/pydanny
.. _`@kennethlove`: https://github.com/kennethlove

Note
----

django-crispy-forms supports Django 1.3 or higher with Python 2.6.x, Python 2.7.x and Python 3.3.x. If you need to support Python 2.5 or Django 1.2 you will need to use a version of django-crispy-forms less than 1.3. For earlier versions of Django or Python you will need to use django-uni-form 0.7.0.

.. _Django: http://djangoproject.com
