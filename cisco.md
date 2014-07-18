% Cisco Curriculum - Zusammenfassung
% 18.07.2014

# 1 Introduction to Routing and Packet Forwarding

## Router:

* verantwortlich für die Auslieferung von Paketen über verschiedene Netzwerke. Dazu gehört es
	* den besten Pfad ausfindig zu machen und
	* Pakete weiterzuleiten
* müssen Pakete entpacken und (in ein eventuell andersartiges Paket) verpacken

### Hardware des Routers

* CPU
* RAM; speichert:
	* OS
	* Running Configuration File (`running-config`)
	* IP Routing Table
	* ARP Cache
	* Packet Buffer
* ROM; speichert (bei Cisco-Routern):
	* bootstrap instructions
	* grundlegende Diagnosesoftware
	* vereinfachte Version von IOS
* Flash Memory; speichert:
	* OS
* NVRAM (Nonvolatile RAM); speichert (bei Cisco-Routern):
	* Startup Configuration File (`startup-config`)

### Cisco Internetwork Operating System (IOS)

* multitasking-fähig

#### Bootvorgang

1. POST
	* Selbsttest (testet Hardware)
	* Diagnoseprogramme (im ROM gespeichert) werden ausgeführt
2. Bootstrap-Programm laden
	* Bootstrap von ROM in RAM kopieren und ausführen
	* Hauptaufgabe: IOS finden und in den RAM laden
3. IOS finden und laden
	* IOS ist üblicherweise im Flash gespeichert, kann aber auch auf einem TFTP (Trivial File Transfer Protocol) Server gespeichert werden
	* Wenn kein (oder ein unvollständiges) IOS Image gefunden werden kann, wir eine vereinfachte Version aus dem ROM geladen
		* Diese Version kann verwendet werden um Probleme zu diagnostizieren
4. Startup Configuration File finden und laden oder in den `setup-mode` wechseln
	* enthält:
		* Interface-Adressen
		* Routing-Informationen
		* Passwörter
		* Alle anderen Konfigurationen, die vom Netzwerkadministrator vorgenommen wurden
	* wird als `running-config` in den RAM kopiert
	* Wenn keine `running-config` vorhanden ist, wird gefragt, ob in den `setup-mode` gewechselt werden soll
		* Wenn nicht in `setup-mode` gewechselt wird, wird eine default `running-config` verwendet

`Router#show version` (kann verwendet werden um die grundsätzliche Hard- und Software zu überprüfen)

**Weiter bei 1.1.5 Router Interfaces**

# 2 Timm

# 3 Ahmed

# 4 Ahmed

# 5 Leo

# 6 Yunus

# 7 Leo

# 8 Yunus
