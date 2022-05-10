Open edX Demo theme
===================

Theming customizations for the Open edX Demo site:

- Add default organization to course creation form: users can create course only in the `Public` organization.
- Remove Course Access request process from the CMS template: the user already has permissions
  (see openedx-demo-plugin for more information).
- Show in home/catalog courses different than public to protect the image of the site (given the public access).


How to use
==========

.. code-block:: bash

  git clone https://github.com/eduNEXT/openedx-demo-theme.git \
  "$(tutor config printroot)/env/build/openedx/themes/openedx-demo-theme"

  tutor images build openedx

  tutor dev settheme openedx-demo-theme

  tutor dev run watchthemes
