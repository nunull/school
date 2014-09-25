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

[](res/inft/2014-09-25-skizze-01.png)

(fehlt)

----

**25.09.2014**


