#############
Release Notes
#############


.. release-0.0.5

*****************************
0.0.5 (Alpha, in development)
*****************************

In development.

.. release-0.0.4

*************
0.0.4 (Alpha)
*************

Released on July 29, 2011.

* Support for InlineAdmin, all credits for this go to Kristian Oellegaard.

.. release-0.0.3

*************
0.0.3 (Alpha)
*************

Released on May 26, 2011.

* Replaced our ghetto fallback querying code with a simplified version of the
  logic used in Bert Constantins `django-polymorphic`_, all credit for our now
  better FallbackQueryset code goes to him.
* Replaced all JSON fixtures for testing with Python fixtures, to keep tests
  maintainable.
* Nicer language tabs in admin thanks to the amazing help of Angelo Dini.
* Ability to delete translations from the admin.
* Changed nani.admin.TranslatableAdmin.get_language_tabs signature.
* Removed tests from egg.
* Fixed some tests possibly leaking client state information.
* Fixed a critical bug in nani.forms.TranslatableModelForm where attempting to
  save a translated model with a relation (FK) would cause IntegrityErrors when
  it's a new instance.
* Fixed a critical bug in nani.models.TranslatableModelBase where certain field
  types on models would break the metaclass. (Many thanks to Kristian
  Oellegaard for the fix)
* Fixed a bug that prevented abstract TranslatableModel subclasses with no
  translated fields.


.. release-0.0.2

*************
0.0.2 (Alpha)
*************

Released on May 16, 2011.

* Removed language code field from admin.
* Fixed admin 'forgetting' selected language when editing an instance in another
  language than the UI language in admin.


.. release-0.0.1

*************
0.0.1 (Alpha)
*************

Released on May 13, 2011.

* First release, for testing purposes only.


.. _django-polymorphic: https://github.com/bconstantin/django_polymorphic
