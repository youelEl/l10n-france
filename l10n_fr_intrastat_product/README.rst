=====
EMEBI
=====

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:e31636ac5ffe766e7171b8531d14ecc93e2c162d625a250888f605f9dc92cad4
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fl10n--france-lightgray.png?logo=github
    :target: https://github.com/OCA/l10n-france/tree/16.0/l10n_fr_intrastat_product
    :alt: OCA/l10n-france
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/l10n-france-16-0/l10n-france-16-0-l10n_fr_intrastat_product
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runboat-Try%20me-875A7B.png
    :target: https://runboat.odoo-community.org/builds?repo=OCA/l10n-france&target_branch=16.0
    :alt: Try me on Runboat

|badge1| |badge2| |badge3| |badge4| |badge5|

This module adds support for the *Enquête mensuelle statistique sur les échanges de biens intra-UE* (EMEBI), for France. Before 2022, this declaration was called Déclaration d'Échange de Biens (DEB).

More information about the EMEBI is available on this `official web page <https://www.douane.gouv.fr/fiche/reglementation-sur-la-reponse-lenquete-mensuelle-statistique-sur-les-echanges-de-biens-intra>`_.

**Table of contents**

.. contents::
   :local:

Configuration
=============

To configure this module, you need to:

 * go to the menu Invoicing > Configuration > Intrastat > Transaction Types to create/verify the Transaction Types
 * go to the menu Invoicing > Settings and go to the *Intrastat* section

Make sure that you have already configured the other modules *intrastat_base* and *intrastat_product* on which this module depends.

WARNING: there are A LOT of settings for DEB and all these settings need to be configured properly to generate DEBs with Odoo.

Usage
=====

To use this module, you need to go to the menu Invoicing > Reports > Intrastat > EMEBI and create a new EMEBI. Depending on your obligation levels, you may have to create 2 EMEBIs: one for departures (Expéditions) and one for arrivals (Introductions). Then, click on the button *Generate lines from invoices* to automatically generate the computation lines of EMEBI. After checking the lines that have been automatically generated, click on the button *Confirm* to generate the declaration lines, create the XML file and set the declaration readonly. Eventually, connect to your account on `douane.gouv.fr <https://www.douane.gouv.fr/>`_ and upload the EMEBI XML file.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/l10n-france/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/OCA/l10n-france/issues/new?body=module:%20l10n_fr_intrastat_product%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Akretion

Contributors
~~~~~~~~~~~~

* Alexis de Lattre <alexis.delattre@akretion.com>

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

.. |maintainer-alexis-via| image:: https://github.com/alexis-via.png?size=40px
    :target: https://github.com/alexis-via
    :alt: alexis-via

Current `maintainer <https://odoo-community.org/page/maintainer-role>`__:

|maintainer-alexis-via| 

This module is part of the `OCA/l10n-france <https://github.com/OCA/l10n-france/tree/16.0/l10n_fr_intrastat_product>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
