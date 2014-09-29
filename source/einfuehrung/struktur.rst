========
Struktur
========

.. |date| date:: %d.%m.%Y
.. |time| date:: %H:%M

:Authors: - Purodha Blissenbach
:Date: |date|, |time|

Die technische Struktur bei Hostsharing aus Anwendersicht:

:Hostsharing:
	- betreibt mehrere Hosts
:ein Host:
	- enhält Null oder mehr Hives
:ein Hive:
	- *liegt auf genau einem Host*
	- enthält Null oder mehr Pakete
:ein Paket:
	- *liegt auf* genau einem Hive
	- hat genau einen Paket-Admin
	- hat genau eine Paket-Domain
        - hat Null oder mehr weitere Unix-Nutzer (neben dem Paket-Admin)
        - hat Null oder mehr E-Mail-Aliases
        - hat Null oder mehr Domains
        - hat Null oder mehr Datenbank-Nutzer
        - hat Null oder mehr Datenbanken
        - hat mindestens einen SSL-Schlüssel und eine IPV4-Adresse
:ein Unix-Nutzer:
	- *gehört zu* genau einem Paket
	- hat genau eine Mailbox
	- kann ein Paket-Admin sein
	- kann ein Domain-Admin sein
	- kann einen Shell-Zugang haben
:eine Domain:
	- *liegt in* genau einem Paket
	- *gehört* genau einem Domain-Admin (möglicherweise dem Paket-Admin)
	- hat eine oder mehrere E-Mail-Adressen
	- hat Null oder mehr Subdomains
:eine Datenbank:
	- *gehört zu* genau einem Paket
	- erlaubt Zugriffsrechte für Null oder mehr Datenbank-Nutzer
:ein Datenbank-Nutzer:
	- *gehört zu* genau einem Paket
	- hat Zugriffrechte auf Null oder mehr Datenbanken
