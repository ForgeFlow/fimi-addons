.. image:: https://img.shields.io/badge/licence-LGPL--3-blue.png
    :alt: License LGPL-3

Purchase Request
================

You use this module if you wish to give notification of requirements of
materials and/or external services and keep track of such requirements.

Requests can be created either directly or indirectly. "Directly" means that
someone from the requesting department enters a purchase request manually.

The person creating the requisition determines what and how much to order,
and the requested date.

"Indirectly" means that the purchase request initiated by the application
automatically, for example, from procurement orders (MO, SO).

A purchase request is an instruction to Purchasing to procure a certain
quantity of materials services, so that they are available at a
certain point in time.

A line of a requisition contains the quantity and requested date of the
material to be supplied or the quantity of the service to be performed. You
can indicate the service specifications if needed.

Once request is approved go to the Purchase Request Lines from the menu entry
'Purchase Requests', and also from the 'Purchase' menu.

Select the lines that you wish to initiate the RFQ for, then go to 'More'
and press 'Create RFQ'.

You can choose to select an existing RFQ or create a new one. In the later,
you have to choose a supplier.

In case that you chose to select an existing RFQ, the application will search
for existing lines matching the request line, and will add the extra
quantity to them, recalculating the minimum order quantity,
if it exists for the supplier of that RFQ.

In case that you create a new RFQ, the request lines will also be
consolidated into as few as possible lines in the RFQ.

Configuration
=============

To configure the product follow this steps:

#. Go to a product form.
#. Go to *Inventory* tab.
#. Check the box *Purchase Request* along with the route *Buy*.

With this configuration, whenever a procurement order is created and the supply
rule selected is 'Buy' the application will create a Purchase Request instead
of a Purchase Order.

Usage
=====

Purchase requests are accessible though a new menu entry 'Purchase
Requests', and also from the 'Purchase' menu.

Users can access to the list of Purchase Requests or Purchase Request Lines.

It is possible to filter requests by its approval status.

.. image:: https://odoo-community.org/website/image/ir.attachment/5784_f2813bd/datas
   :alt: Try me on Runbot
   :target: https://runbot.odoo-community.org/runbot/142/11.0

For further information, please visit:

* http://www.eficent.com/blog_en/streamline-your-purchasing-process-in-odoo-using-purchase-requests/


Bug Tracker
===========

Bugs are tracked on `GitHub Issues
<https://github.com/OCA/purchase-workflow/issues>`_. In case of trouble, please
check there if your issue has already been reported. If you spotted it first,
help us smashing it by providing a detailed and welcomed feedback.


Credits
=======

Images
------

* Enric Tobella (logo)


Contributors
------------

* Jordi Ballester Alomar <jordi.ballester@eficent.com>
* Jonathan Nemry <jonathan.nemry@acsone.eu>
* Aaron Henriquez <ahenriquez@eficent.com>
* Adrien Peiffer <adrien.peiffer@acsone.eu>
* Lois Rilo <lois.rilo@eficent.com>
* Héctor Villarreal Ortega <hector.villarreal@eficent.com>

Maintainer
----------

.. image:: http://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: http://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

To contribute to this module, please visit http://odoo-community.org.
