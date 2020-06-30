# Meesterproef Product Bio
![Happy Flow van de ticketstraat](https://user-images.githubusercontent.com/33430655/84995585-79f5bc80-b14c-11ea-849b-a1d1b169dc70.gif)

## Inhoudsopgave
- [Github repository & design rationale]()
- [Het team]()
- [Debriefing & presentaties]()
- [Communicatie]()

## Github repository & design rationale 
- [Repository](https://github.com/Mokerstier/Rijksmuseum-Ticketflow)
- [Design rationale](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/wiki/Design-rationale)
- [Prototype](https://rijks-ticket-flow.herokuapp.com/)

## Het team
- [Mohamad Al Ghorani](https://github.com/MohamadAlGhorani)
- [Manouk Kappé](https://github.com/ManoukK)
- [Wouter van der Heijde](https://github.com/Mokerstier)

## Debriefing & presentaties 
- [Mijn eigen debriefing](https://github.com/Mokerstier/meesterproef-1920/wiki/Debriefing)
- [Presentatie debriefing (PDF)](https://github.com/ManoukK/meesterproef-1920/files/4818881/Debriefing.pdf)
- [Eind presentatie (PDF)](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/wiki/Laatste-presentatie)

## Communicatie
- Discord (screensharing en (video-)gesprekken)
- Slack Minorweb (we hadden ons eigen kanaal waar dingen afspraken)
- Slack Q42 (hier werden we geïnformeerd over meetings met de opdrachtgever)

## Mijn rol
Ik had in mijn groepje het meeste ervaring met github daarom hebben we er samen voor gekozen dat ik de repo zou aanmaken en behere. Hierbij heb ik verantwoording genomen met het opzetten van een project board, en het zetten van milestones. Bij iedere "nieuwe" actie waarvan ik wist dat mijn team niet op de hoogte was van deze functionaliteit heb ik ze in een video-call (met screensharing) uitgelegd wat ik deed.
Samen met Mohamad heb ik mij gefocussed op het technische gedeelte van de opdracht. Desondanks hebben we zoveel mogelijk geprobeerd om elkaar te betrekken bij grote onderdelen van het prototype. Het idee hierachter is dat iedereen inzicht krijgt wat er gebeurd op de server. Een opssoming van enkele projecten onder mijn verantwoordelijkheid:

- Github setup (inclusief project board, planning & branche protection)
- :pencil: Recording & notuleren van de user tests
- Basis HTML geschreven voor de verschillende stappen
- :pencil: .csv bestanden omzetten naar werkbaar .json
- :pencil: [Plan van aanpak](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/wiki/Plan-van-aanpak)
- :bug: Bugfixes
- :pencil: Research naar ARIA

### Dingen die niet gelukt zijn:
- Polyfill inzetten voor cross-browser support (babel)
- Op de datum picker stap lay-out aanpassen op de stap in het proces (meer info in [Schetsen - UX-Datepicker]())

## Het process
De samenwerking ervaarde ik persoonlijk als zeer prettig. Doordat we met issues werkte werd het voor iedereen inzichtelijk waar kern-problemen waren en hoe, en vooral wie, deze ging oplossen. We keken per dag naar de issues en indien nodig loste we deze samen op. De communucatie in het team verliep nagenoeg perfect. We hielden elke dag contact en zaten dan bijna de hele (werk)dag in een call (via discord). Ook het contact met de opdrachtgever was goed, de feedback die we kregen a.d.v. de demo's die we gaven was constructief en doordacht. Hiermee hebben ze ons erg geholpen.

## Planning
Onze planning liep geheel via github - projects. De grote features of taken kregen een label: high-prio. Waardoor we belangerijke van minder belangrijke issues konden onderscheiden en zo dus prioriteit konden geven aan de verschillende issues.

## Een gemiddelde werkdag
We kwamem 's ochtends rond een uur of 10 samen op discord en bespraken eventuele progressie aan issues en planning voor de dag. Meestal resulteerde dit in intensieve gezamelijke code-sessies door middel van screensharing. Aan het einde van de dag kwamen we meestal nog even samen om de dag door te spreken. Hoe het was gegaan en welke problemen waren ontstaan of verholpen.


## Leerdoelen
Voor dit project heb ik mijzelf de volgende leerdoelen gesteld:

1. Toegankelijkheid
   #### Zorg dat de applicatie volledig toegankelijk is voor alle gebruikers.
   Op het gebied van toegankelijkheid heb ik vooral gewerkt aan een toegankelijke datum-kiezer.
   W3C heeft wat zei zelf noemen een "accesible-datepicker" gemaakt maar deze kwam niet overeen met onze eigen ideeën. Wij hebben uiteindelijk gekozen voor een andere aanpak. We hebben de datum-kiezer opgedeelt in stappen, met een vraag antwoord spel. Door deze aanpak hebben wij een datum-kiezer kunnen maken die geheel toegankelijk is waarbij de gebruiker nooit een *"*verkeerde"* datum kan kiezen. Uit verschillende tests en iteraties is de datum-kiezer geworden zoals hij nu is. Onze (blinde) test-personen zeiden het volgende: "Ik denk niet dat het het meest snelle design is om door heen te gaan, maar je zorgt er zo wel voor dat het voor iedereen werkt en nooit mis gaat!" - Jesse Wienholts.
   Ook gaf hij tijdens de test al aan dat hij het een prettige interface vond.

   >  De gebruiker krijgt alleen opties diie beschikbaar zijn.

    #### Geef feedback aan de gebruiker wanneer dit nodig is.
    Ook hebben we veel gedaan met feedback. Zo hebben we gebruik gemaakt van aria-live regions om de bestellinglijst met onze gebruikers te delen wanneer deze verandert. Meer hierover is terug te lezen in de design rationale: [Aria - live](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/wiki/Wat-kunnen-wij-gebruiken-om-het-toegankelijker-te-maken-(met-aria)#aria-live).

    #### Geef feedforward om de gebruiker te helpen met bestelproces.
    Per stap in het process met name bij de datum kiezer, geven we instructies aan de gebruiker hoe hij/zij dit gedeelte van het formulier kan bedienen. Tijdens de testen met Roger & Hannes kwamen wij erachter dat het voor hen soms nog onduidelijk was hoe zij het formulier moesten bedienen. Hierop hebben wij instructies geschreven zoals: "Navigeer door de selectie met uw pijltjes toetsen", "Selecteer uw keuze met de spatie-balk". Dit werd in latere tests als prettig ervaren door onze kandidaten.

2. Testen

   Ik heb voor ons team contact gezocht met Roger Raveli, waar ik al eerder mee had gewerkt tijdens het vak WEB-Design. Roger stond te springen om met ons aan de slag te gaan en was erg nieuwsgierig naar onze bevindingen. Via school en Q42 zijn wij ook nog in contact gebracht met Hannes Walraven en Jesse Wienholts. Tijdens het testen heb ik gezorgd voor een test-omgeving (google - meet) en ben ik verantwoordelijk voor het notuleren van deze tests. Later heb ik de bevindingen met mijn team gedeeld waarna we een conclusie hebben geformuleerd en problemen omgezet naar issues op het project board.

   >Er is gebruikt gemaakt van milestones om de bevindingen (issues) uit de tests te bundelen en inzichtelijk te maken. Een voorbeeld van zo'n milestone vind je hier: [Link naar milestone testfase 1](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/milestone/6?closed=1).

3. Browser Tech

   #### Local-storage
   Door niet alleen feature detectie toe te passen op de local storage maar ook een simpele test uit te voeren weten we of de local-storage beschikbaar is en of deze niet is uitgeschakeld door de gebruiker.
   ```
   function localStorageTest() {
      const test = "test";
      try {
        localStorage.setItem(test, test);
        localStorage.removeItem(test);
        return true;
      } catch (e) {
        return false;
      }
    }
   ```
   We weten nu als `localStorageTest()`, `true` terug geeft dat we hem kunnen gebruiken.

   #### Flow zonder javascript
   Op de client doen we veel met javascript met name in de datum-kiezer. Maar omdat javascript niet altijd werkt of uit staat. Is er gezorgd voor een alternatieve flow die geheel zonder javascript werkt. De ervaring van de gebruiker zal iets anders zijn maar het belangrijkste is dat de gehele ticket-straat nog steeds goed werkt!

4. Modulairiteit en schaalbaarheid
   Dit project is opgezet met het idee dat de opdrachtgever onze gemaakte feautures als module's kan integreren in het betsaande ontwerp. Zo werken we met een echte dataset en is onze applicatie hieromheen gebouwd. Doordat de content allemaal dynamisch wordt inladen is het voor de opdrachtgever eenvoudig om content toe te voegen of te verwijderen zonder dat de applicatie stuk gaat. Hierdoor is ons prototype uitstekend schaalbaar en goed te onderhouden

## Reflectie


<!-- Add a link to your live demo in Github Pages 🌐-->

<!-- ☝️ replace this description with a description of your own work -->

<!-- Add a nice poster image here at the end of the week, showing off your shiny frontend 📸 -->

<!-- Maybe a table of contents here? 📚 -->

<!-- How about a section that describes how to install this project? 🤓 -->

<!-- ...but how does one use this project? What are its features 🤔 -->

<!-- Maybe a checklist of done stuff and stuff still on your wishlist? ✅ -->

<!-- How about a license here? 📜 (or is it a licence?) 🤷 -->
