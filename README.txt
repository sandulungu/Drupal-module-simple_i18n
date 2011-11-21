
The Simple I18n module implements a trivial patter matching markup to enclose
your localizable strings. Anything that is sent to the user using a theme page
template (and is not published in the /admin section) gets parsed by this
module, so when the markup is found it is automatically filtered and outputted
in the current language.

Why was it created?
===================

The main difference form the existing I18n suite (that I tried to use and did
not work out as expected for menus, taxonomy and views):

* this module is trivial to setup and covers all the needs left over by the
  content translation module for small sites.
* it uses a simple to understand (and easy to type) syntax, that should be safe
  for usage in output ( a "[[@ ... ; ... ; ... ]]" is not common IMHO neither
  for JS, CSS, HTML, XML or human/machine-readable content. I consider allowing
  configuration of the pattern, if required by the comunity.

Compatibility
=============

It's for Drupal 7.x (but can easily be ported to 6.x).
