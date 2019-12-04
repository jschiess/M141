# Modul 141 individuelles Projekt
## Arbeitsjournal
### Grobbeschrieb
	Es soll für die aktuelle Todo-App Projekt einen Benutzer Login erstellt werden. Dazu das Datenbank Schema mittels knex kreiert werden.

	Zur Datenbank soll hinzugefügt werden:
	Mykek.owner soll ein verschlüsseltes Passwort bekommen.
	Man sollte nur ein Todo unter seinen eigenen Name kreieren, löschen und ändern können.
### Mittel und Methode
#### Frontend
* Vue
	* Vuetify

* Axios

#### Backend
* Express
* Knex
* jsonwebtoken
* Bcrypt

#### Vorarbeit
Das Projekt: Todo-App.

#### Neue Kenntnisse
##### Vertiefung in
* JWT
* Bcrypt
* loginverfahren

### Arbeitsjournal

#### Tag 1
* Datenbank angepasst 
	* zur tabbelle user eine neuen Attribut password hinzugefuegt.
	* fuelldaten angepasst.
	* hashen des passworts erfolgt mit bcrypt v 3.0.0
* login path erstellt
	* JWT brauchen /login
	* /login returnt Bearer Auth token
#### Tag 2
* logger erstellt, welcher die zeit und path logged
	* evt. noch den user logged
	* evt. noch die daten in eine file speichern
* Files aufgesplittet um Modularitaet zu gewinnen
* bug fixes und code verschloenert
* frontend anpassen
	* views erstellen
	 	* /login | die seite aufder man kommt wenn man nicht eingeloggt ist bzw. ein invaliden token hat
#### Tag 3
	* kleine UI anpassungen
	* bug fix mit todos erstellen
	* migration user_group erstellt.
		* foreign key zu group und user erstellt

	* notes
		* bei mysql muessen beide relationen in einer constraint signed sein
		* bei knex werden increments() automatisch auf unsigned gesetzt

### todo 
	* presentation vorbereiten
	* gruppen implimentation



### Fragen an marco
* wieso ist cors noetig?