======================
HSAdminmodul mysqluser 
======================

.. |date| date:: %d.%m.%Y
.. |time| date:: %H:%M

:Authors: - Uwe Müller
          - Dominic Schlegel

:Date: |date|, |time|


Das HSAdminmodul ``mysqluser`` verfügt über folgende Optionen:



+---------------+------------------------------------------------+
| Option        | Erläuterung                                    |
+===============+================================================+
| name          | Name des Datenbanknutzers (z.B. xyz00_abc)     |
+---------------+------------------------------------------------+
| password      | Password                                       |
+---------------+------------------------------------------------+

Beispiel:

.. code-block:: console

    $ mysqluser.add  ({set:{name:'xyz00_owner',password:'!1?2-3aBc'}})
 
