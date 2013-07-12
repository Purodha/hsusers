========
Accounts
========

:Authors: - Uwe Müller
:Date: 2013-03-01

Accounts
========

Für unterschiedliche Aufgaben und Rechte der User in einem Paket hat Hostsharing eine Terminolgie vergeben um
die zugedachten Aufgaben und Rollen zu verdeutlichen.  Die Trennung erfolgt durch die Vergabe
von Rechten auf der Betriebsystemebene. User werden mit dem Administrationstool HSadmin (http://hsadmin) verwaltet.

Die Hierarchie gliedert sich in absteigender Reihenfolge.

TODO: zeichen und längenbeschränkung der usernamen.

Mitgliedsaccount 
================

- Initial vorhanden
- der Name ist xyz (hsh00-xyz)
- hat keine Shell (das Programm "passwd" wird an Stelle einer Shell gestartet).
- erlischt mit dem Ende der Mitgliedschaft
- eigenes Passwort
- technisch unabhängig von anderen Accounts

Nutzung
=======

- mit HSAdmin alle Pakete verwalten
- Passwörter der Paket-Admins ändern
- kann die Rechte eines Paket-Admins annehmen
- Rechnungen herunterladen
- technisch unabhängig von anderen Accounts

Domainbestellsystemaccount
==========================

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

alle Rechte eines [anker: Domain-Admins] und folgende zusätzliche Rechte:

- Domains einem User (Domainadmin) des Pakets zuordnen,
- Domains des Paketes administrieren,
- User und Datenbanken einrichten, löschen und ändern,
- per "sudo -u xyz00-paketuser -i" die Rechte eines Users seines Paketes annehmen.

note::
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

- E-Mail-Adressen für eine Domain einrichten,
- Sub-Domains anlegen,
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
