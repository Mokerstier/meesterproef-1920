# Meesterproef Product Bio
![Happy Flow van de ticketstraat](https://user-images.githubusercontent.com/33430655/84995585-79f5bc80-b14c-11ea-849b-a1d1b169dc70.gif)

## Inhoudsopgave
- [Github repository & design rationale](https://github.com/Mokerstier/meesterproef-1920/)
- [Het team](https://github.com/Mokerstier/meesterproef-1920/)
- [Debriefing & presentaties](https://github.com/Mokerstier/meesterproef-1920/)
- [Communicatie](https://github.com/Mokerstier/meesterproef-1920/)
- [Mijn rol](https://github.com/Mokerstier/meesterproef-1920/)
- [Het proces](https://github.com/Mokerstier/meesterproef-1920/)
- [Planning](https://github.com/Mokerstier/meesterproef-1920/)
- [Gemiddelde werkdag](https://github.com/Mokerstier/meesterproef-1920/)
- [Leerdoelen](https://github.com/Mokerstier/meesterproef-1920/)
- [Reflectie](https://github.com/Mokerstier/meesterproef-1920/)

## Github repository & design rationale 
- :tada:[Repository](https://github.com/Mokerstier/Rijksmuseum-Ticketflow)
- :pencil:[Design rationale](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/wiki/Design-rationale)
- :rocket:[Prototype](https://rijks-ticket-flow.herokuapp.com/)

## Het team :busts_in_silhouette:
- [Mohamad Al Ghorani](https://github.com/MohamadAlGhorani)
- [Manouk Kappé](https://github.com/ManoukK)
- [Wouter van der Heijde](https://github.com/Mokerstier)

## Debriefing & presentaties 
- [Mijn eigen debriefing](https://github.com/Mokerstier/meesterproef-1920/wiki/Debriefing)
- [Presentatie debriefing (PDF)](https://github.com/ManoukK/meesterproef-1920/files/4818881/Debriefing.pdf)
- [Eind presentatie (PDF)](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/wiki/Laatste-presentatie)

## Communicatie :speech_balloon:
- Discord (screensharing en (video-)gesprekken)
- Slack Minorweb (we hadden ons eigen kanaal waar dingen afspraken)
- Slack Q42 (hier werden we geïnformeerd over meetings met de opdrachtgever)

## Mijn rol :building_construction:
Ik had in mijn groepje het meeste ervaring met github daarom hebben we er samen voor gekozen dat ik de repo zou aanmaken en beheren. Hierbij heb ik verantwoording genomen met het opzetten van een project board, en het stellen van milestones. Bij iedere "nieuwe" actie waarvan ik wist dat mijn team niet op de hoogte was van deze functionaliteit heb ik ze in een video-call (met screensharing) uitgelegd wat ik deed.
Samen met Mohamad heb ik mij gefocussed op het technische gedeelte van de opdracht. Desondanks hebben we zoveel mogelijk geprobeerd om elkaar te betrekken bij grote onderdelen van het prototype. Het idee hierachter is dat iedereen inzicht krijgt wat er gebeurd op de server en hoe bepaalde code werkt. Een opssoming van enkele projecten onder mijn verantwoordelijkheid:

- :pencil: Github setup (inclusief project board, planning & branche protection)
- :pencil: Recording & notuleren van de user tests
- Basis HTML geschreven voor de verschillende stappen
- :pencil: .csv bestanden omzetten naar werkbaar .json
- :pencil: [Plan van aanpak](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/wiki/Plan-van-aanpak)
- :bug: Bugfixes
- :pencil: Research naar ARIA

### Wishlist:
- Polyfill inzetten voor voleedige cross-browser support (babel)
- Op de datum picker stap lay-out aanpassen op de stap in het proces (meer info in [Schetsen - UX-Datepicker]())

## Het proces
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
   W3C heeft wat zei zelf noemen een "accesible-datepicker" gemaakt maar deze kwam niet overeen met onze eigen ideeën. Wij hebben uiteindelijk gekozen voor een andere aanpak. We hebben de datum-kiezer opgedeelt in stappen, met een vraag antwoord spel. Door deze aanpak hebben wij een datum-kiezer kunnen maken die geheel toegankelijk is waarbij de gebruiker nooit een *"*verkeerde"* datum kan kiezen. We hebben gedurende het proces de vragen iets verder uitgebreid door de uiteindelijk opties bij het kiezen van een tijd te halveren (van 20 keuzes naar 10). De reden hiervoor was om de gebruiker niet te overspoelen met mogelijkheden. Uit verschillende tests en iteraties is de datum-kiezer geworden zoals hij nu is. Een van onze test-personen zei er het volgende over: "Ik denk niet dat het het meest snelle design is om door heen te gaan, maar je zorgt er zo wel voor dat het voor iedereen werkt en nooit mis gaat!" - Jesse Wienholts.
   Ook gaf hij tijdens de test al aan dat hij het een prettige interface vond.

   >  De gebruiker krijgt alleen opties die beschikbaar zijn.

    #### Geef feedback aan de gebruiker wanneer dit nodig is.
    Ook hebben we veel gedaan met feedback. Zo hebben we gebruik gemaakt van aria-live regions om de bestellinglijst met onze gebruikers te delen wanneer deze verandert. Meer hierover is terug te lezen in de design rationale: [Aria - live](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/wiki/Wat-kunnen-wij-gebruiken-om-het-toegankelijker-te-maken-(met-aria)#aria-live).

    #### Geef feedforward om de gebruiker te helpen met bestelproces.
    Per stap in het process met name bij de datum kiezer, geven we instructies aan de gebruiker hoe hij/zij dit gedeelte van het formulier kan bedienen. Tijdens de testen met Roger & Hannes kwamen wij erachter dat het voor hen soms nog onduidelijk was hoe zij het formulier moesten bedienen. Hierop hebben wij instructies geschreven zoals: "Navigeer door de selectie met uw pijltjes toetsen", "Selecteer uw keuze met de spatie-balk". Dit werd in latere tests als prettig ervaren door onze kandidaten.

2. Testen
   #### Regel test kandidaten en faciliteer een user-test.
   Ik heb voor ons team contact gezocht met Roger Raveli, waar ik al eerder mee had gewerkt tijdens het vak WEB-Design. Roger stond te springen om met ons aan de slag te gaan en was erg nieuwsgierig naar onze bevindingen. Via school en Q42 zijn wij ook nog in contact gebracht met Hannes Walraven en Jesse Wienholts. Tijdens het testen heb ik gezorgd voor een test-omgeving (google - meet) en ben ik verantwoordelijk voor het notuleren van deze tests. Later heb ik de bevindingen met mijn team gedeeld waarna we een conclusie hebben geformuleerd en problemen omgezet naar issues op het project board.

   >Er is gebruikt gemaakt van milestones om de bevindingen (issues) uit de tests te bundelen en inzichtelijk te maken. Een voorbeeld van zo'n milestone vind je hier: [Link naar milestone testfase 1](https://github.com/Mokerstier/Rijksmuseum-Ticketflow/milestone/6?closed=1).

3. Browser Tech

   #### Zet local-storage in om de gebruiker de kans te geven zijn bestelling op een ander moment af te maken.
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

   #### Zorg dat de gebruiker de gehele ticket-flow kan doorlopen ook als javascript uit staat.
   Op de client doen we veel met javascript met name in de datum-kiezer. Maar omdat javascript niet altijd werkt of uit staat. Is er gezorgd voor een alternatieve flow die geheel zonder javascript werkt. De ervaring van de gebruiker zal iets anders zijn maar het belangrijkste is dat de gehele ticket-straat nog steeds goed werkt!

4. Modulairiteit en schaalbaarheid
   #### Zorg ervoor dat het project schaalbaar is en te implementeren door de opdrachtgever.
   Dit project is opgezet met het idee dat de opdrachtgever onze gemaakte feautures als module's kan integreren in het betsaande ontwerp. Zo werken we met een echte dataset en is onze applicatie hieromheen gebouwd. Doordat de content allemaal dynamisch wordt inladen is het voor de opdrachtgever eenvoudig om content toe te voegen of te verwijderen zonder dat de applicatie stuk gaat. Hierdoor is ons prototype uitstekend schaalbaar en goed te onderhouden

## Reflectie
Binnen dit project lag de focus voornamelijk op toegankelijkheid. Daarom zijn sommige vakken minder of helemaal niet aan bod gekomen. Zo zou er bijvoorbeeld meer aandacht besteed kunnen worden aan multi-user support. Er wordt nu nog gebruik gemaakt van enkele globale variabelen waardoor ons prototype nu voor 1 gebruiker geschikt is gemaakt. In de toekomst zou ik misschien wat meer tijd besteden aan sessions om deze variablen op te slaan. Ook wordt er nog geen data gemanipuleerd door de gebruiker. De reden dat we ervoor hebben gekozen dit soort dingen niet uit te voeren was omdat in het orginele ontwerp van Q42 deze facetten al goed zijn uitgewerkt. Bovendien zou het veel tijd kosten om dit soort onderdelen grondig uit te werken en die tijd steek ik liever in het goed ontwerpen en testen van de toegankelijkheid; wat overigens door de opdrachtgever als kern-probleem werd benoemd. In het begin van het project zijn we zo snel mogelijk begonnen met bouwen, omdat we de dataset van het rijksmuseum wouden gebruiken, daarna hebben we het ontwerp zoals we het gebouwd hadden weer aangepast aan de hand van schetsen. Dit was omdat we de gehele flow van de ticketstraat hebben aangepast. Ondanks dat dit niet heel veel tijd koste zou ik in de toekomst eerder gaan schetsen en daarna pas gaan bouwen. Het liefst zou ik door middel van sockets multi-user support willen bieden en daadwerkelijk een ticket reserveren vanuit de beschikbaar gestelde data van het Rijksmuseum. Maar tevens door tijdgebrek is er gekozen om dit niet te doen. We hebben veel onderzoek gedaan naar browser support en hebben zelfs een alternatieve flow gecreëerd voor mensen zonder javascript. Desondanks is het niet gelukt om ons prototype geschikt te maken voor alle browsers. De problemen liggen vooral bij wat nieuwere functionaliteiten zoals: `scrollIntoView()`, `closest()`, `fetch()` idealiter zouden hier beter fallbacks voor egschreven moeten worden. Vooral IE gaf de meeste problemen omdat deze de nieuwe functionaliteiten niet goed ondersteund. Vooralsnog gaat het protoype dus stuk in deze browser, maar met meer tijd en research moet ook het geschikt maken voor deze browsers geen probleem meer zijn. Dit is in iedergeval een punt waar ik in de toekomst nog meer naar wil gaan kijken. (De huidige ticket-straat van het Rijksmuseum heeft al onwijs slechte ondersteuning in oudere browsers). We hebben nauwlijks tijd besteed aan performance. Wel is er gebruikt gemaakt van verschillende buildscripts, zowel css als js, om de critical render path iets te optimailseren. In een toekomstig project is dit ook nog een punt waar ik meer aandacht aan wil besteden. Wat betreft web design is er werkelijk tot het maximale gedaan om te zorgen voor een goede UX voor mensnen met een visuele beperking (denk aan eerder benoemde, Feedback, Feedforward, en is er geprobeerd om de gebruiker zoveel mogelijk te helpen). Er is onwijs veel tijd besteed aan deze doelgroep omdat dit vanuit de opdrachtgever als zeer belangrijk werd bestempeld. Desalniettemin is er zo veel mogelijk voor gezorgd om voor iedereen te ontwerpen en voor iedereen een prettige ervaring aan te bieden. Aan de hand van alle positieve reacties van zowel, docent, opdrachtgevers en test kandidaten denk ik dat dit uitstekend is gelukt! Met veel plezier heb ik dan ook aan dit project gewerkt en ik heb genoten van de samenwerking met mijn team. Wij hebben ieder op een gelijkwaardig niveau samengewerkt waarin ieders kwaliteiten optimaal zijn benut.

