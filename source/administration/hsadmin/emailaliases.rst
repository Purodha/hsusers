=========================
HSAdminmodul emailaliases 
=========================

.. |date| date:: %d.%m.%Y
.. |time| date:: %H:%M

:Authors: - Uwe Müller

:Date: |date|, |time|


Das HSAdminmodul ``emailaliases`` verfügt über folgende Optionen:

+---------------+----------------------------------------------------------------------+
| Option        | Erläuterung                                                          |
+===============+======================================================================+
| name          | Name des E-Mailalias                                                 |
+---------------+----------------------------------------------------------------------+
| target        | Ziel einer E-Mail-Adresse, mehrere Ziele werden durch Komma getrennt |
+---------------+----------------------------------------------------------------------+

Beispiel:

.. code-block:: console

    $ emailalias.add ({set:{name:'xyz00',target:'webmaster@hs-example.de'}})

