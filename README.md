> _Fork_ deze leertaak en ga aan de slag. Onderstaande outline ga je gedurende deze taak in jouw eigen GitHub omgeving uitwerken. De instructie vind je in: [docs/INSTRUCTIONS.md](docs/INSTRUCTIONS.md)

# 🎨 Keep Users in Control Activity Diagram
<!-- Geef je project een titel en schrijf in één zin wat het is -->
Activity Diagram voor de MijnHvA applicatie.

## 🍿 User Story
<!-- Schrijf hier de User Story waar de Activity Diagram over gaat-->
Als gebruiker, wil ik een aantal fetch states zien (loading state, error state & empty state), zodat ik weet dat de API werkt.

## 🎸 Activity Diagram
<!-- Toon de activity Diagram -->
![Acticity Diagram](https://github.com/JustinLung/keep-users-in-control-activity-diagram/blob/main/docs/activity-diagram.png?raw=true)

## 🖥 Uitleg pseudo-code 
<!-- Leg de pseudo-code in de control fow uit -->
In mijn activity diagram is te zien hoe de content van de pagina wordt geladen in modules. Tijdens het project van de MijnHvA App, gaan wij in modules werken. Hierbij heb ik dus een activity diagram uitgewerkt met behulp van [✍️ draw.io](https://app.diagrams.net/). 

- App.js is mijn startpunt (hier wordt alle hoofdcode ingeladen)
- wanneer Javascript uitstaat, krijg je een empty state. Hierbij is dan op het scherm te zien dat je je Javacript aan moet zetten. (De swimlane)
- vervolgens na de app.js roepen wij de api.js aan waarbij de functie getData wordt aangeroepen.
- na het aanroepen van de getData functie, wordt de state loading aangeroepen. Hierbij wordt er een spinner getoond op de applicatie. Dat is een indicator voor als de content nog aan het laden is.
- Als dit niet lukt, wordt er een error message laten zien. Deze error message is de error state. (Swimlane)
- als de fetch succesvol is, dan wordt de api gefetched en wordt de state loaded getoond.
- na het fetchen van de data, wordt de render functie aangeroepen, waar de content van de applicatie wordt gerendered

## 🤌 Licentie

![GNU GPL V3](https://www.gnu.org/graphics/gplv3-127x51.png)

This work is licensed under [GNU GPLv3](./LICENSE).
