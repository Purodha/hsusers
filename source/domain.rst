======
Domain
======

:Authors: - Uwe Müeller
:Date: 2013-03-01

Domain-Aktionen
---------------

Bei Hostsharing sind folgende Aktionen mit Domains möglich:
 
- Domainregistrierung/-transfer zu Hostsharing
- Domainkündigung (Transfer zu einem anderen Provider)
- Extern registrierte Domains/Subdomains bei Hostsharing aufschalten
- Domain/Subdomains neu zuordnen (Domain-Admin, Paketzuordnung ändern)
- lokale Subdomains separat aufschalten
- Domain löschen
- eigene Verwaltung der Zonefiles

Domainverwaltung
----------------

Die Domainverwaltung  ist in zwei Bereiche aufgeteilt:

- Domaineinrichtung und -konfiguration.
  Die Einrichtung und Konfiguration wird mit HSadmin auf der shell (http:// hsadmin-shell)
  oder Alternativ im Webfrontend (http:// hsadmin webfrontend) durchgeführt.


- Domain-Bestellsystem (http:// doku-domainbestellsystem)
  Zur Vergabe von Aufträgen (Registrierung, Kündigung, Transfer) an Domainregistrierungsstellen.

  Die Vergabe von Aufträgen an Domainregistrierungsstellen ist nur über das Webfrontend möglich.
  Der Nutzer ist für die Aktionen im Domainbestellsystem juristisch eigenverantwortlich.  Über das Webfrontend
  sind, abhängig von der jeweiligen Domainregistrierungsstelle, sämtliche  Aktionen möglich
  wie z.B. Registrierung, Update von Benutzerdaten, Änderungen von DNS-Servern, CHPROV (change provider, KK), Kündigung und Transit einer Domain.
  Die Anzahl der pro Tag möglichen Registrierungen ist auf 25 Domains beschränkt, um den Nuzter vor Mißbrauch zu schützen.

Paket-Subdomain xyz00.hostsharing.net
-------------------------------------

Bei der Paketeinrichtung wird die Subdomain xyz00.hostsharing.net automatisch im doms-Ordner
angelegt. Hierbei handelt es sich um eine nutzbare Subdomain, die alle Funktionen von Domains unterstützt
mit folgenden Einschränkungen:

- Die Paket-Subdomain kann nicht gelöscht oder einem anderen Benutzer zugeordnet werden.
- Subsubdomains zu der Paketdomain können nicht aufgeschaltet werden.
- Das Zonefile der Paket-Subdomain sollte auf keinen Fall geändert werden, da durch 
  Änderungen am Zonefile der Paket-Subdomain das gesamte Paket nicht mehr funktionsfähig sein kann.

Die Paket-Subdomain ist dafür geeignet, Webpakete oder Web-Anwendungen zu testen ohne das
hierfür eine Domain registriert werden muss. 
