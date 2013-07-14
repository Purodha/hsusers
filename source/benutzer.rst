========
Benutzer
========

:Authors: - Uwe Müller
:Date: 2013-07-13




Benutzer
========

Für unterschiedliche Aufgaben der Benutzer in einem Paket können unterschiedliche Rollen vergeben werden, die durch die Vergabe
von Rechten auf Betriebsystemebene definiert werden. 

Die Hierarchie gliedert sich in absteigender Reihenfolge.

TODO: zeichen und längenbeschränkung der usernamen.

Mitglied 
========

- Initial vorhanden
- der Name ist xyz 
- hat keine Shell
- erlischt mit dem Ende der Mitgliedschaft
- eigenes Passwort
- technisch unabhängig von anderen Benutzern

Nutzung
=======

- mit HSAdmin alle Pakete verwalten die dem Mitglied zugeordnet sind
- kann die Rechte eines Paket-Admins annehmen
- Rechnungen herunterladen
- technisch unabhängig von anderen Accounts

Domainbestellsystem
===================

- Initial vorhanden
- der Name ist hs-xyz
- eigenes Passwort

Nutzung
-------

- Login in das externe	Domainvertrags-Verwaltungstool

Paket-Admin
===========

- ist Initial vorhanden.
- der Name ist xyz00 (http:// pakete).
- hat eine reguläre Shell (z.B. "/bin/bash")
- weitere User beginnen mit dem Paket-Präfix xyz00-, gefolgt von einer individuell zu vergebenen
  Zeichenfolge.
- hat einen E-Mail Account

Nutzung
-------

- verwaltet ein Web-Paket, seine User, Dienste und Domains. 

Rechte
------

alle Rechte eines Domain-Admin und folgende zusätzliche Rechte:

- Domains einem User (Domainadmin) des Pakets zuordnen,
- Domains des Paketes administrieren,
- User und Datenbanken einrichten, löschen und ändern,
- kann die Rechte eines Users seines Paketes annehmen.

``note``
    Eine Domain kann auf den Account eines Paketadmins aufgeschaltet werden.
    Aus Sicherheitsgründen empfiehlt es sich Domains auf separate User aufzuschalten.

Domainbestellungen siehe Domainbestellungen

Domain-Admin
============

- wird durch den Paket-Admin angelegt
- hat eine reguläre Shell (z.B. "/bin/bash")
- hat eine Verzeichnisstruktur unterhalb ~/doms/
- hat einen E-Mail Account

Nutzung
------- 

Verwalter seiner Domain(s)

- Sub-Domains aufschalten
- Dateien und Verzeichnisse anlegen oder ändern


Rechte
-------

- E-Mail-Adressen für eine Domain einrichten
- Sub-Domains anlegen
- Zonen-Daten einer Domain bearbeiten.


User ohne Shell
===============

- wird durch den Paket-Admin angelegt,
- hat keine Shell (das Programm "passwd" wird an Stelle einer Shell gestartet).


Nutzung
-------

- als E-Mail-Account.

Rechte
------

- es kann nur das Passwort geändert werden.


Datenbank-User
==============

Die Datenbank-Systeme haben jeweils ihre eigene User-Verwaltung. (http:// Datenbankuser)

Verwaltung der User (http:// userverwaltung http:// hsadmin shell http:// hsadmin webfrontend)
