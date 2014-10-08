# Telekommunikation

## Begriffe

### Verbindungsorientiert

1. Verbindungsaufbau
2. Datenübertragung
3. Verbindungsabbau

#### Möglichkeiten

* **Wählverbindung**: Verbindung der Kommunikationspartner für eine gewisse Zeit.
	* Herstellung einer Leitungsverbindung (leitungsvermittelt) **oder**
	* Nachricht wird in einzelne Pakete unterteilt und (eventuell) über verschiedene Leitungswege zugestellt (paketvermittelt, zellorientiert)
* **Festverbindung** (Standleitung): Zwei Kommunikationspartner sind dauerhaft miteinander verbunden.

### Verbindungslos

* Nur Phase der Informationsübertragung (siehe oben)
	* Stationen senden spontan Datenpakete (Nutzdaten mit Ursprungs- und Zieladresse)
	* Zielstation entniimmt dem Datenstrom, die an sie adressierte Info

\newpage

## Anschlüsse

| **ISDN-Basisanschluss** | | 
|-|-|
| **Mehrgeräteanschluss** | **Anlagenanschluss** |
| NTBA als Netzabschluss | NTBA als Netzabschluss |
| NTBA + Endgeräte (Telefone, Fax, etc.) | NTBA + Telefonanlage + Endgeräte |
| | |
| 8 ISDN-Geräte pro S0-Bus | <- dito, jedoch für jeden S0-Bus |
|  jedoch maximal 4 Telefone | |
| 1 S0-Bus | |
| 12 IAE-Dosen | |
| | |
| Netzanbindung über eine CU-Doppelader | <- dito |
|  (USTP) | Sonderfall: Einige TK-Anlagen bieten |
| | die Möglichkeit mehrerer externer S0-Busse. |
| | Für jeden externen S0-Bus wird 1 NTBA |
| | benötigt (vgl Skizze 1) |
| | |
| **TN-Seite**: | |
| 1 S0-Bus (4-adrig), passiver Bus -> keine | Anzahl S0-Busse von TK-Anlage abhängig |
| Verstärker und Regeneratorelement | |
| | |
| 2 B-Kanäle je 64 kbit/s | extern: 2 B-Kanäle |
| 1 D-Kanal 16 kbit/s | 1 D-Kanal |
| 160 kbit/s Übertragungsrate | intern: B+D-Kanäle entsprechend der|
| | TK-Anlage |



| **Primärmultiplexanschluss** |
|-|
| **Anlagenanschluss** |
| NTPM als Netzabschluss |
| NTPM + Telefonanlage + Endgeräte |
| |
| Anzahl Geräte / Dosen wie bei *Basis-Anlagenanschluss* (siehe oben) |
| **TN-Seite** wie bei *Basis-Anlagenanschluss* (siehe oben) |
| Netzanbindung über zwei CU-Doppeladern **oder** Koax **oder** LWL |
| |
| extern: 30 B-Kanäle je 64 kbit/s |
| 1 D-Kanal 64 kbit/s |
| Synchronisationskanal 64 kbit/s |
| intern: wie bei *Basis-Anlagenanschluss* (siehe oben) |
| 2048 kbit/s Übertragungsrate |

\newpage

**17.09.2014**

## AB 1

### Aufgabe 2

*Was wird in der Telekommunkationstechnik mit der UK0-Schnittstelle und was mit der S0-Schnittstelle bezeichnet?*

Der Begriff **UK0-Schnittstelle** bezeichnet die Schnittstelle eines ISDN-Basisanschlusses, die verwendet wird, um den *Vermittelnden Netzknoten* (NVK) mit dem *NTBA* zu verbinden. Das U steht hierbei für den Referenzpunkt der Schnittstelle im  *ISDN-Referenzmodell*. das K steht für Kupfer und die Null bezeichnet den ISDN-Basisanschluss.

Der Begriff **S0-Schnittstelle** bezeichnet die Schnittstelle eines ISDN-Basisanschlusses, die verwendet wird, um ISDN-Endgeräte mit dem NTBA zu verbinden. Der S0-Bus wird hausintern verwendet.

#### Lösung:

##### S0-Schnittstelle / -Bus:

**Teilnehmer-(TN-)seitige** Schnittstelle zwischen NTBA und Endgerät (TN); Referenzpunkt auf TN-Seite

##### UK0-Schnittstelle:

**Netzseitige** (Netzbetreiber) Schnittstelle zwischen VST (Vermittlungsstelle) und NTBA; Referenzpunkt auf Netzseite

### Aufgabe 3

*Welche Anschlusskonfigrationen stehen bei einem ISDN-Anschluss zur Verfügung und worin unterscheiden sie sich im Wesentlichen?*

...

### Aufgabe 4

*Warum muss der S0-Bus terminiert werden und in welcher Weise wird die Terminierung in der Praxis durchgeführt?*

Der S0-Bus muss **terminiert** werden, um Reflektionen, bzw. Störungen auf den Leitungen zu vermeiden. In der Praxis werden 100 Ohm Widerstände verwendet. Die Terminierung findet an jedem Ende des S0-Busses zwischen Sende- und Empfangsleitung statt. Es sind also pro Ende des Busses jeweils zwei Widerstände notwendig. Im NTBA sind diese schon vorhanden. Am anderen Ende ist der einfachste Weg zur Terminierung der Einsatz von IAE-Dosen mit integrierten schaltbaren Widerständen.

#### Lösung:

Reflexionen vermeiden; Terminierung an beiden Enden mit jeweils einem 100 Ohm Widerstand; R ist in NTBA, IAE, UAE

### Aufgabe 5

#### a) / b)

*Wie viele ISDN-Endgeräte dürfen laut Spezifikation maximal an die Teilnehmerschnittstelle des NTBA angeschlossen werden?*

*Wie viele ISDN-Aschlussdosen dürfen maximal an den S0-Bus angeschlossen werden?*

An der Teilnehmerschnittstelle des NTBA dürfen maximal zwölf Anschlussdosen und acht Endgeräte angeschlossen werden.

##### Lösung:

*a)*: 8 (maximal 4 Telefone); *b)*: 12 Anschlussdosen IAE

#### c)

*Wie viele Telefongespräche könnten die Mitarbeiter gleichzeitg und unabhängig voneinander über das ISDN führen?*

Im Falle eines ISDN-Basisanschlusses können zwei Telefongeräte parallel geführt werden (so lange nicht gleichzeitig ein Fax oder Daten übertragen werden).

##### Lösung:

2 Gespräche pro Basisanschluss

30 Gespräche beim Primärmultiplexanschluss

#### d)

*Lassen sich an den S0-Bus auch vorhandene Telefone anschließen? Wenn ja, dann erstelle eine Skizee und erkläre diese. Wenn nein, dann begründe Deine Antwort und zeige eine Alternative auf.*

An den S0-Bus lassen sich direkt keine analogen Telefone anschließen. Hierfür ist ein so genannter *A/B-Wandler* (*Terminaladapter*; *TA*) notwendig. Der *A/B-Wandler* setzt die analogen Signale des Telefons als digitale ISDN-Signale um (und umgekehrt).

##### Lösung:

Ja, allerdings mit einem *Terminaladapter* (*TA*; *A/B-Wandler*)

#### e)

*An welcher Stelle erfolgt die Analog- / Digitalumsetzung der Signale, wenn bei einem ISDN-Basisanschluss analoge Telefone eingesetzt werden?*

Die Analog- / Digitalumsetz erfolgt zwischen *UAE-Dose* (*S0-Bus*) und analogem Gerät im *A/B-Wandler* (*Terminaladapter*; *TA*).

----

**24.09.2014**

(fehlt; nachtragen!)

Siehe Skizze 1

----

**25.09.2014**

## DSL-Anschluss

Siehe Skizze 2

Die DSL-Technik ermöglicht eine  schnelle digitale Datenübertragung auf herkömmlichen Kupferleitungen. Höhere Datenraten werden durch einen höheren Frequenzbereich (DSL: 1,1 MHz / ISDN: 120 kHz) erreicht.

* Die eigenen Frequenzbereiche von DSL und ISDN ermöglichen, dass beide parallel auf **einer** Leitung übertragen werden können.
* DSL-Splitter zerlegen bzw. trennen als Frequenzweiche das Signal in DSL- und ISDN-Datenströme und leiten jedes an die Endgeräte (DSL-Modem bzw. ISDN-NTBA) weiter.

----

**26.09.2014**

## Nachtrag zum NTBA bzw. $U_{k0}$ und $S_0$

### 1) Kanalcodierung der $U_{k0}$-Schnittstelle

* *4B/3T*-Code oder auch *MMS43*-Code
* für Übertragung auf TN-Aschlussleitung $U_{k0}$
* Datenstrom wird in 4-Bit-Blöcke (*4B*) aufgeteilt.
* jeder Block wird in ein 3-Schritt-Tenärsignal (*3T*) umgewandelt.
* 4B/3T_code hat vier verschiedene Alphabete (Status 1-4), Auswahl des Folgestatus hängt von gerade vorher codierten 3T-Wort ab.

### 2) Kanalcodierung der $S_0$-Schnittstelle

* Sende- und Empfangsrichtung sind durch 4-Drahtbetrieb voneinander getrennt
* Es kommt ein *modifizierter AMI-Code* zum Einsatz, dabei werden "0"-Bits als Impuls, "1"-Bits als Impulslücke übertragen

#### Beispiel AMI

	Info:       0 1 0 0 1 1 0 0 0 1
	AMI-Signal: - 0 + - 0 0 + - + 0 (modifizierter AMI-Code)

(`0`-Bits werden als Impuls, `1`-Bits als Impulslücke übertragen.)

## Hausaufgabe bis zum 30.10.2014 (PCM)

### Aufgabe 1

*Was ist die wesentliche Aufgabe der PCM-Technik? Erkläre.*

* (Umsetzung eines zeit- und wertkontinuirlichen Analogsignals als zeit- und wertdiskretes Digitalsignal)
* Übertragung von Signalen über weite Strecken
* durch Zeitmultiplexen eine Übertragungsstrecke mehrfach nutzen

### Aufgabe 2

*Welches sind die wesentlichen drei Schritte bei der Digitalisierung? Nenne diese.*

1. Abtastung des Signals durch *Pulsamplitudenmodulation*
2. Quantisierung auf diskrete Werte
3. Codierung

### Aufgabe 3

*Erläutere den Grund für die nichtlineare Quantisierungskennlinie.*

(Geringeres Quantisierungsrauschen pro Bit als bei linearer Quantisierung)

Bei kleinen Spannungen würden sich größere Ungenauigkeiten ergeben als bei größeren Spannungen.

### Aufgabe 4

*Erkläre stichwortartig, wie die eindeutige Zuordnung der 8-Bit-Wörter zu den jeweiligen Kanälen ermöglicht wird.*

feste, immer gleichbleibende zeitliche Zuordnung der 8-Bit-Wörter (Zeitschlitz) innerhalb eines pulsrahmens

### Aufgabe 5

*Erläutere stichwortartig den Aufgabe eines PCM-30 Pulsrahmens.*

(Pulsrahmen legt den Aufbau der zu sendenden Daten fest.)

* 32 Kanäle, davon 30 Kanäle für Datenübertragung
* Kanal 16 beinhaltet Kennzeichen der 30 TN
* Kanal 0 beinhaltet Meldewörter (Rahmentrennung, Synchronisation)
* PCM-30-Pulsrahmen ist 125$\mu\text{s}$ lang, mit je 8 Bit; Einteilung der 125$\mu\text{s}$ in 32 Zeitschlitze

----

**02.10.2014**

## Aufgaben

### Aufgabe 1

#### a)

**Beschreibe die plesiochrone digitale Hierarchie und die synchrone digitale Hierarchie.**

##### Plesiochrone digitale Hierarchie (PDH)

* basiert auf dem PCM-Übertragungssystem
* PDH weißt eine Multiplexstruktur auf, die auf Übertragungsraten mit ganzzahligen Vielfachen von 64 kbit/s aufbauen.
* hierbei werden die Datenkanäle zu Pulsrahmen mit jeweils fest vorgegebenen Übertragungsraten zusammengefasst.

##### Synchrone digitale Hierarchie (SDH)

* Übertragung der Nutzdaten erfolgt zwischen den einzeönen Netzknoten **nicht** mehr in einer Rahmenstruktur mit fest vorgegebenener Anzahl von Kanälen, die jeweils eine konstante Bitrate aufweisen müssen, **sondern** in dem so genannten synchronen Transportmodulen (STM: Synchronous Transport Module). Unter einem Transportmodule versteht man einen Multiplexrahmen der SDH, in dem Nutzdaten von mehreren Kanälen, die auch unterschiedliche Datenrahmen aufweisen können, übertragen werden. *STM1* ist das kleinste Transportmodul.

**Vorteil** SDH gegenüber PDH:

Übertragungssysteme mit unterschiedlichen Übertragungsraten können kombiniert werden. SDH ermöglicht den Zugriff auf Signale bestimmter Bandbreite innerhalb eines hochkanäligen Systems ohne die gesamte Multiplexstruktur durchlaufen zu müssen.

#### b)

**Welche der beiden Standards ist zu bevorzugen? Begründe deine Antwort.**

SDH (siehe a)

### Aufgabe 2

#### a)

**Erkläre das Prinzip des asynchronen Transfer-Modus. Wie funktioniert die Übertragung? Was passiert, wenn von den Teilnehmern zu viele bzw. zu wenig Zellen angeliefert werden?**

Beim ATM werden - ähnlich wie beim *Packet Transfer Mode* (PTM) - "Packete" übertragen. Diese Packete haben jedoch eine konstante Länge.

#### b)

**Was versteht man bei einem ATM-Netz unter dem flexiblen Bandbreitenmanagement?**

ATM stellt einer Anwendung oder einem Dienst lediglich die tatsächlich erforderliche Übertragungskapazität zur Verfügung. Dies bezeichnet man als flexibles Bandbreitenmanagment.

#### c)

**Welcher Vorgang ist bei ATM asynchron?**

Zellen werden *asynchron* zum Netztakt erzeugt und bedarfsorientiert übertragen.

#### Zusatz

##### Synchronous Transfer Mode (STM)

Beim STM werden Daten in festern Zeitschlitzen mit einer bestimmten Bandbreite übertragen. Zwischen Endgeräten ist - unabhängig vom Bedarf dieser - immmer eine feste Bandbreite verfügbar.
