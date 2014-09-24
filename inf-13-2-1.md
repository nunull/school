% Informatik - Unterrichtsmitschriften
% Timm Albers
% 20.06.2014 - 15.07.2014

# XML

## XML Namensräume

* xmlns-Attribut
	* Standnamensraum
* xmlns:xxx-Attribut
	* left den Namensraum xxx fest (Definition eines Kürzels)
* Definitionen sind für alle untergeordneten Tags und für das definierende Tag gültig. Namespaces müssen weltweit eindeutig sein. Hierfür wird daher i.d.R. eine URL verwendet.

### Beispiel

	<root xmlns="http://www.szut.de/bsp1"
	      xmlns:xxx="http://www.szut.de/bsp2">
	      
		<xxx:bla><!-- bla aus dem NS xxx -->
			Hallo Welt!
		</xxx:bla>
	</root>
	
## Aufgabe

Erstellen Sie eine XSD für das Schachbrett (Beispiel vom letzten Mal) anhand der der Informationen unter [http://www.w3schools.com/schema](http://www.w3schools.com/schema)

