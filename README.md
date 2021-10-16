## **Oefeningen: In memory web API & Routing**
### Oefening 1
Voorzie een nieuwe Angular applicatie met de naam ch9-oefening1 in de root directory van deze repository met 3 components. In de app.component.html voorzie je 3 hyperlinks: Home, Info, getallen. En een inputbox waarin de waarde via 2way binding gekoppeld wordt aan een variabele “getal”.

Voorzie volgende routes & functionaliteit:
*   De Home component bevat tekst (lorem ipsum) en wordt getoond onder de navigatie bij het laden van de url /home. Daarnaast wordt de base url ([http://localhost:4200/](http://localhost:4200/)) doorverwezen naar deze component
*   De Info component bevat ook tekst (lorem ipsum) en een knop. Deze knop wijzigt de waarde van de boolean clicked uit de component. De waarde staat standaard op false. De gebruik kan deze view enkel verlaten als de waarde van clicked true is. (canDeactivate)
*   De getallen component krijgt een parameter mee in zijn route als volgt: getal/5. Deze parameter is in de link in de navigatie gelijk aan het getal uit de inputbox. In de component view wordt de tafel van het meegegeven getal weergegeven. 

Controleer na het maken van deze oefening of je alle wijzigingen naar github hebt gepusht.

### Oefening 2
Maak een nieuw angular project met als naam h9-oefening2 in de root directory van deze repository.

**De routing van deze oefening voorzie je in een aparte routing module! **Voorzie een angular applicatie met onderstaande functionaliteit. Een service met een array van Events (id, titel, datum, adres) en de methodes getEvents(), getEvent(id), addEvent(event), removeEvent(id).

*   Een component create-event. In deze component voorzie je een eenvoudig formulier voor het toevoegen van een event. (Route: /create)
*   Een component event-list. Hierin toon je een lijst van alle events uit de array. Je kan op elke event klikken om de event-detail component in te laden. (Route: /list). Deze component wordt geladen bij het starten van de app (Route: /)
*   Een component event-detail. Hierin toon je de details van een event in een div. **De data van de event wordt via een resolver opgehaald.** Indien de event niet terugkomt in de array (dus een foute id in de route), redirect je naar de 404 pagina.
*   Een component error-404. Indien je een route bezoekt die niet bestaat, wordt deze component getoond. (Route: /404)
*   Voorzie in de lijst een delete knop. Bij het klikken verwijs je naar de route remove/:id. De remove component heeft een melding “Event deleted” en delete de event in de ngOnInit methode. Vooraleer je de component toont, geef je een melding “Are you sure?” (canActivate).

Controleer na het maken van deze oefening of je alle wijzigingen naar github hebt gepusht.

### Oefening 3

Ga naar de map H9-oefening-debug. Vervolgens run je onderstaand commando in deze map op alle dependencies te installeren:

npm install
In dit project zitten verschillende fouten. Probeer aan de hand van de error messages in je IDE & developer console de fouten weg te werken zodat je een werkende applicatie krijgt.

Controleer na het maken van deze oefening of je alle wijzigingen naar github hebt gepusht.
