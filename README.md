# GIP website van Thom Ernst

##### Welkom in het github repository van mijn website!
- - -
__Wat kan je vinden in deze versie van mijn website?__

* __Een _index.html_ dat linkt naar alle andere documenten met een responsief menu, deze pagina's laden dan in een iframe__
    * De enige webpagina die eigenlijk wordt bezocht, al de rest gebeurt via iframes
* __Intro__
* __Lijst met GIP-taken__
* __Over Mezelf__
* __IT-tapa__
* __Stage__
* __Disco__
* __Game__
   
* __CSS__
_____
    * Veel css komt van _Pure_

    * Maakt gebruik van font awesome voor een reeks incoontjes
    
    * Gebruik van grids voor bepaalde afbeeldingen, voornamelijk aangepast met _Pure_

    * Deels geen gebruik van ``px`` in de opmaak

    * Vervangen door ``em`` als relatieve lengte

    * Aangepaste versie van de "_dynamic button and responsive menu_" css voor persoonlijke stijl
    
    * De folder vendor is een locatie waar ik alle bestanden steek die ik link in mijn website, maar die niet van mezelf zijn of aangepast zijn, dus van 3den
    
    * Animate.css wordt gebruikt en is een library dat allerlei ``onload`` animaties voorziet
    
    * Daarbovenop is er een class ``wobble-vertical`` die buttons en andere elementen tot leven brengt
    
    * ## Links:
     * [main.css](https://github.com/ThomE-immalle/GIP-Website/blob/master/ccs/main.css)
     * [Responsive side-menu](https://github.com/ThomE-immalle/GIP-Website/blob/master/ccs/main.css#L145)
     * [vendor](https://github.com/ThomE-immalle/GIP-Website/blob/master/vendor)

* __HTML__
_____
    * de inhoud van elke pagina wordt gedisplayed in een iframe ipv aparte html bestanden
    
    * html5 elementen zoals ``head``, ``main``, ``footer``, ``nav``, en nog wat andere items
    
    * placeholder tekst zal worden aangevuld naargelang gip-taken worden afgemaakt
    
    * elementen in het responsive-menu linken naar de iframe-bestanden, sommige gebruiken font-awesome, andere iconen zijn zelf gemaakt
    
    * de game past live de inhoud van het iframe aan, als je [het spel](http://3d.wolfenstein.com/game/wolf3d.html) bekijkt in de inspector kan je helemaal zien hoe het spel reageert met de html
    
* __JS__
 * Responsief zij-menu [MenuJS](https://github.com/ThomE-immalle/GIP-Website/blob/master/js/MenuJs.js)
 * Er zit javascript en jquery in de disco module, ik heb deze niet zelf geschreven, maar wel helemaal doornomen. Ik heb hier veel uit bijgeleerd (vooral de jquery dom structuur)
 * Er zit javascript in het spel, deze heb ik ook doornomen, het interessante is dat bijna alles in een apart .js bestand zit, elke control, functie...
 * Het It-Profile wordt gemaakt met een google chart volledig in javascript deze ziet er zo uit: 
                ```javascript
                    google.charts.load('current', {'packages':['corechart']});
                    google.charts.setOnLoadCallback(drawChart);
                    function drawChart() {
                        var data = google.visualization.arrayToDataTable([
                            ['onderdeel 1', 'percentage'],
                            ['deel',           45],
                            ['deel',       55],
                        ]);
                        var options = {
                            title: 'titel'
                        };
                        var chart = new google.visualization.PieChart(document.getElementById('id-van-element'));
                        chart.draw(data, options);
                    } 
                ```

## Dingen die ik kwijt wil over het maken van mijn website

* Op zoek gaan naar een font die goed past in het design van een website is moeilijk, maar gewoon standaard arial gebruiken is ook altijd saai, ik ga in de toekomst zeker nog met een paar fonts experimenteren op mijn website

* Ik ben van plan om in de toekomst zelfgemaakte _svg_'s toe te voegen op de website per GIP-project, als een soort van aanvulling op mijn opleiding van digitaal tekenen

* Ik ben lang bezig geweest om alle bestanden te linken met https, uiteindelijk heb ik gewoon een domein aangemaakt en gebruikt mijn website http

* De disco -en game-modules heb ik toegevoegd omdat ik vond dat de website niet genoeg respresenteerde hoe ik zelf ben, ze zijn er dus om de plaats een beetje op te beuren en om mezelf te motiveren om verder aan deze website te werken

## Updatelist

* 8/11
 * een andere achtergrond afbeelding en ervoor gezorgd dat deze niet verdwijnt of te veel verandert met herschalen browser
 * favicon toegevoegd
 * probleem met de sidebar die een scrollbar vertoonde
* 20/11
 * iframe gebruikt om de content op te laden ipv aparte html bestanden
 * afbeelding gecompresseerd
 * To-Do: buttons met iframe linken
* 21/11
 * bewerkingen aan het iframe-systeem
 * readme herbekeken en issues opgelost
 * html5-elementen toegevoegd (header, main, footer)
* 27/11
 * Branch merge tussen master en de testbranch
  * Disco toegevoegd
  * Game toegevoegd
  * Readme geupdate
  * IT-profile gemaakt
  * IT-tapa pagina-sjabloon aangemaakt
* 29/11
 * Smoothscroll toegevoegd
 * To top buttons aangemaakt
 * tweaks aan index.html
* 2/11
 * ###Dit is een late update van de readme maar het omvat ongeveer wat ik deze week nog gedaan heb
 * animaties aan allerlei elementen wanneer ze inladen of wanneer de muis erover gaat
 * stage-pagina heeft een sjabloon
 * IT-tapa pagina is afgewerkt
 * aanpassingen aan de takenlijst - deze zal in de toekomst linken naar alle projecten
 * link naar Axel zijn website was verkeerd, dit is opgelost
 * ``hr`` elementen toegevoegd voor betere visuele details
 * v1.0 definitief afgewerkt
