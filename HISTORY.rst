Changelog
=========

1.16.0 (2016-04-25)
~~~~~~~~~~~~~~~~~~~

* Minor bugfix for fields-from-model handling of auto fields


1.15.0 (2016-04-21)
~~~~~~~~~~~~~~~~~~~

* Table.from_model implemented


1.14.0 (2016-04-19)
~~~~~~~~~~~~~~~~~~~

* Added `after` attribute on `Column` to enable custom column ordering (See `tri.declarative.sort_after()`)

* Enable mixing column definitions in both declared fields and class meta.

* Don't show any results if the form is invalid


1.13.0 (2016-04-08)
~~~~~~~~~~~~~~~~~~~

* Add python 3 support


1.12.0 (2016-02-29)
~~~~~~~~~~~~~~~~~~~

* Changed syntax for specifying html attributes and classes. They are now use the same way of addressing as
  other things, e.g.: Column(attrs__foo="bar", attrs__class__baz=True) will yield something like
  `<th class="baz" foo=bar>...</th>`


1.11.0 (2016-02-04)
~~~~~~~~~~~~~~~~~~~

* Fix missing evaluation of row__attr et al.


1.10.0 (2016-01-28)
~~~~~~~~~~~~~~~~~~~

* Changed cell__template and row__template semantics slightly to enable customized cell ordering in templates.

  row__template implementations can now access a BoundCell object to use the default cell rendering.

  cell__template implementation are now assumed to render the <td> tags themself.


1.9.0 (2016-01-19)
~~~~~~~~~~~~~~~~~~

* Fixed to work with latest version of tri.form
