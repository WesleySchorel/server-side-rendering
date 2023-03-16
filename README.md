![image](https://user-images.githubusercontent.com/112857487/225697241-a06e366e-31a8-46e9-8024-922d1443eb40.png)

# Vervoerregio Amsterdam (Server-side-rendering)

## Inhoudsopgave

  * [Beschrijving](#beschrijving)
  * [Kenmerken](#kenmerken)
  * [Installatie](#installatie)
  * [Gebruik](#gebruik)
  * [Bronnen](#bronnen)
  * [Licentie](#licentie)

## Beschrijving
Vervoerregio Amsterdam wilt een website waarop een overzicht van de verplichtingen voor toegankelijkheid van website's bekeken kunnen worden. Aan de hand van deze criteria die op de website te vinden zal zijn kan Vervoerregio Amsterdam haar partners controleren op toegankelijkheid.

De twee userstories die ik heb uitgevoerd zijn:
> 1. Als gebruiker wil ik een overzicht van toegankelijkheidsrichtlijnen kunnen bekijken, om te begrijpen wat er moet gebeuren om een website/app toegankelijker te maken.

> 2. Als gebruiker wil ik detail informatie over een toegankelijkheidsrichtlijn bekijken, om te beoordelen of mijn website/app voldoet aan de richtlijn.

https://doubtful-sweatpants-dog.cyclic.app/

## Kenmerken
Deze website is gebouwt met verschillende technologieën. De technologiën die ik heb gebruikt zijn met Node, Express en EJS en een REST API.

### Node
```js
// Maak een route voor de index
app.get('/toolboard', function (req, res) {
  console.log(data)
  res.render('toolboard', {api: data, active: '/toolboard'})
})
```

### Rest API
In dit project maak ik gebruik van de REST API for Toolgankelijkheid van Vervoerregio Amsterdam. De documentatie van deze Api is te vinden op: https://api.vervoerregio-amsterdam.fdnd.nl/

### Express
Express is het framework dat de routing op mijn website regelt.
```js
// Maak een nieuwe express app aan
const app = express()

// Stel ejs in als template engine en geef de 'views' map door
app.set('view engine', 'ejs')
app.set('views', './views')
```

## Installatie
Download of clone dit project van deze Github pagina.

Download de aanbevolen versie op nodejs.org en installeer vanaf deze wwebsite de Node ontwikkelomgeving. Tijdens dit project heb ik gebruik gemaakt van 18.14.0 LTS, download de benodigde bestanden en doorloop het installatieproces van Node.

Open de terminal in Visual Studio Code en installeer Node doormiddel van het commando ``npm init``. Voer hierna ``npm install`` uit. Om de pagina te open start je een server op door middel van ``npm start``. Als de server weer gesloten moet worden kan je ``control + c / ^c`` gebruiken.

## Gebruik
Gebruik van de website zal worden gedaan door de medewerkers van Vervoerregio Amsterdam via deze website kunnen zij de website's van hun partners controleren op de richtlijnen en toegankelijkheid principes die verplicht worden in 20225. 

1. Navigeer naar het toolboard doormiddel van de navigatie bovenaan de pagina of druk op de grote witte knop onder de introtekst. 
2. U belandt op een pagina waarop alle richtlijnen en principes te vinden zijn. Klik op de blauwe knoppen om meer informatie te krijgen over de succescriteria.

## Bronnen
> _Fork_ deze leertaak en ga aan de slag. Onderstaande outline ga je gedurende deze taak in jouw eigen GitHub omgeving uitwerken. De instructie vind je in: [docs/INSTRUCTIONS.md](docs/INSTRUCTIONS.md)

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
