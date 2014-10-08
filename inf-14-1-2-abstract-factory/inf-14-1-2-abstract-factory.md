title: Abstract Factory
output: inf-14-1-2-abstract-factory.html
controls: false
style: style.css

--

# Abstract Factory

## Entwurfsmuster 

--

# Abstract Factory

## Erzeugermuster

--

# Absicht:

--

# 

> "Provide an interface for creating families of related or dependent objects without specifying their concrete classes." 

<center>(Design Patterns, Gamma et al.)</center>

--

# 

> "Abstract Factory soll ein Interface anbieten um Familien von verwandten oder abhängigen Objekten zu erstellen, ohne deren konkrete Klassen anzugeben."

<center>(Design Patterns, Gamma et al.)</center>

--

# 

<center>Hä?</center>

--

# 

<center>Verwandte / abhängige Objekte erstellen</center>

--

# Funktionsweise:

--

### Funktionsweise

* konkrete Factories erben von abstrakter Factory
* Factories haben Factory Methods
	* Rückgabetyp: abstrakte Klasse

--

# Konsequenzen:

--

### Konsequenzen 

* Clients rufen Erzeugermethoden auf, wissen aber nicht, welche konkreten Klassen sie verwenden
* Je nachdem, welche Factory ein Client verwendet, wird er verschiedene Familien konkreter Objekte verwenden.
* Objektfamilien sind austauschbar, ohne das der Client verändert werden muss
* Client bleibt unabhängig
* Abhängigkeiten zwischen Objekten einer Familie werden verstärkt

--

### Konsequenzen

* Das Einführen neuer Produkte wird erschwert.

--

# Anwendungsfälle:

--

### Anwendungsfälle (1)

* ein System soll unabhängig davon bleiben, wie seine Produkte erstellt, komponiert und repräsentiert werden

--

### Anwendungsfälle (2)

* ein System soll mit einer von mehreren Familien von Produkten konfiguriert werden

--

### Anwendungsfälle (3)

* eine Familie verwandter Produktobjekte wurde designed um zusammen benutzt zu werden. Es ist notwendig dies zu bestärken.

--

### Anwendungsfälle (4)

* eine Klassenbibliothek soll nur die Interfaces der Produkte zeigen, nicht aber die Implementationen.

--

# Implementierung:

--

### Implementierung (1)

#### Factories als Singleton

--

### Implementierung (2)

#### Prototype

--

### Implementierung (3)

#### Erweiterbare Factories

--

# Beispiel:

--

### Beipsiel (1)
