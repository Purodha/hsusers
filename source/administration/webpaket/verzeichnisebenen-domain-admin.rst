=============================
Verzeichnisebene Domain-Admin
=============================

.. |date| date:: %d.%m.%Y
.. |time| date:: %H:%M

:Authors: - Uwe Müller

:Date: |date|, |time|

+-----------------+-----------+--------+---------+----------------------------------------------------------------+
| Rechte Schleuse | Nutzer    | Gruppe | Ordner  | Erläuterung                                                    |
+=================+===========+========+=========+================================================================+
| dr-xr-x--T      | httpd     | xyz00  | doms    |   Ablage der im Web-Paket aufgeschaltenen enthaltenen Domains. |
+-----------------+-----------+--------+---------+----------------------------------------------------------------+
| drwx------      | xyz00-abc | xyz00  | Maildir |  Mailordner des Domain-Admin.                                  |
+-----------------+-----------+--------+---------+----------------------------------------------------------------+


Unterhalb des Ordners *doms* und der Domain *example.de* befindet sich die Verzeichnisstruktur für die jeweilige Domain:


+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| Rechte Schleuse | Nutzer    | Gruppe | Ordner      | Erläuterung                                                                                                     |
+=================+===========+========+=============+=================================================================================================================+
| drwxr-xr-x      | xyz00-abc |  xyz00 | cgi         | Ablage externer Software zur Generierung dynamischer Webseiten in einem Webserver.                              |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | cgi-ssl     | Ablage externer Software zur verschlüsselten Generierung dynamischer Webseiten (siehe auch http SSl/TSL).       |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | fastcgi     | Ablage externer Software zur Generierung dynamischer Webseiten in einem Webserver.                              |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | fastcgi-ssl |  Ablage externer Software zur verschlüsselten Generierung dynamischer Webseiten (siehe auch http SSl/TSL).      |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | htdocs      | Ablage für die Daten einer Webseite, wenn diese unverschlüsselt ausgeliefert werden soll.                       |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | subs        | Ablage für Subdomain aus htdocs, wenn diese unverschlüsselt ausgeliefert werden soll.                           |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | htdocs-ssl  | Ablage für die Daten einer Webseite wenn diese verschlüsselt ausgeliefert werden soll (siehe auch http SSL/TLS. |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | subs-ssl    | Ablage für Subdomain aus htdocs-ssl, wenn diese verschlüsselt ausgeliefert werden soll.                         |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | etc         | Ablage für Domaineigene Konfigurationsdateien (z.B. eigenes Zonefile ) http zonefile.                           |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+
| drwxr-xr-x      | xyz00-abc |  xyz00 | var         | Ablage für Logfiles.                                                                                            |
+-----------------+-----------+--------+-------------+-----------------------------------------------------------------------------------------------------------------+



