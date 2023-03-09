# DJ mixer | CSS to the rescue 2023
![banner](https://user-images.githubusercontent.com/94384526/224050849-0164f93d-0535-4825-a4ac-b7e0fb64509a.png)
https://maxvl3.github.io/css-to-the-rescue-2223/
<br> Werkt alleen in Safari Technology Preview (bevat functionaliteiten achter een vlag 🚩)
<br> Het beste te bekijken met een 13 inch scherm

<details>
  <summary>Week 1</summary>
  
  ## Welke opdracht ga je doen en voor welke opties kies je qua uitwerking?
  Ik heb gekozen om te gaan werken aan de modulaire bedieningspaneel case. Ik kreeg bij de presentatie direct al ideeën in mijn hoofd voor eventuele uitwerkingen. Het leek me ook erg interessant om eens te kijken wat je allemaal kunt doen met input velden, in plaats van default styling. Mijn idee voor deze opdracht is om een soort trading software te gaan maken waar je aandelen kan bekijken, kopen en verkopen. (later is dit idee gewijzigd)

  ## Met welke CSS-technieken ga je als eerste aan de slag?
  Door de introductie opdracht heb ik kennisgemaakt met best veel nieuwe css technieken. Een aantal wil ik sowieso gaan proberen te verwerken in mijn eindopdracht, namelijk:
  - Dark/light mode
  - Moderne kleuren (HSL, display-p3)
  - Nesting
  Verder wil ik gaan leren wat ::before en ::after doet en hoe ik het kan gebruiken in mijn opdracht.

  ## Waar liggen je (grootste) uitdagingen?
  Ik denk lastige CSS selectors gebruiken, maar hopelijk kan css nesting mij hierbij helpen.

  ## Neem schets(en) van je ontwerp op
  Hier een eerste digitale schets van mijn concept:
  ![schets1](https://user-images.githubusercontent.com/94384526/224035411-91a17f51-6185-42b1-ad7a-db79a09d68d2.png)
  
  Later ben ik nog geswitcht van idee en heb ik een nieuwe schets gemaakt:
  ![schets2](https://user-images.githubusercontent.com/94384526/224035567-fe1d03f1-af91-4982-9119-f1b3cea00636.png)
</details>

<details>
  <summary>Week 2</summary>
  
  ## Voortgang
  Ik ben begonnen met het maken van een eerste basis in html/css. Mijn dj mixer bestaat uit 3 panelen dus deze heb ik alvast gemaakt samen met 2 schijven en een display. Vanuit hier ga ik later deze week verder met de knoppen.
  ![DJ-mixer](https://user-images.githubusercontent.com/94384526/224037096-c87d08b3-fae1-4f98-8f1d-b9a5b06133b2.png)
  
  Ik ben vervolgens een HI-FI schets gaan maken omdat ik merkte dat ik houvast nodig had tijdens het coderen. Deze heb ik gemaakt in Figma. Ik weet nog niet of dit het uiteindelijke design gaat worden, maar dit is in ieder geval een prima basis.
  ![hifischets](https://user-images.githubusercontent.com/94384526/224037800-cd861d86-05f3-4e05-91a0-f7897098ce80.png)

  Ook heb ik deze week nog een start gemaakt met de knoppen van de dj mixer. Vooral voor nu gefocust op de positionering en kiezen van de juiste HTML elementen.
  ![DJ-mixer (1)](https://user-images.githubusercontent.com/94384526/224038148-c17efcab-cea3-44ff-80d0-8eeeabcadeb7.png)

  ## Wat ging goed wat kon beter?
  | Goed      | Beter |
  | ----------- | ----------- |
  | Duidelijk idee | Nog geen verbeterpunten       |
  | Schetsen gemaakt   |         |
  | Prima start aan code   |         |
  
  ## Wat te doen volgende week?
  Volgende week wil ik zo veel mogelijk styling meegeven aan mijn huidige elementen. Zodat het een wat realistischer dj mixer wordt.
  
</details>

<details>
  <summary>Week 3</summary>
  
  ## Voortgang
  Deze week ben ik ziek geweest, maar desondanks heb ik wel nog wat gewerkt aan de opdracht. Ik ben begonnen met het stylen van het display waar muziekwaves op worden geprojecteerd. Hier heb ik ook een animatie toegevoegd zodat het meer leeft en realistischer wordt.
  ![ezgif com-video-to-gif (1)](https://user-images.githubusercontent.com/94384526/224044989-093d6a05-36c5-487f-9bd5-3403daacde50.gif)
  
  Ook heb ik de draaischijven styling meegegeven en een rotatie animatie hieraan meegeven voor een ronddraaiend effect.
  ![DJ-mixer3](https://user-images.githubusercontent.com/94384526/224045397-2afbc5fd-c502-44e7-b8f7-4bc572338904.png)
  
  ## Wat ging goed wat kon beter?
  | Goed      | Beter |
  | ----------- | ----------- |
  | CSS schrijven | Had graag wat meer willen doen deze week
  | Animaties gemaakt (tijdje geleden voor het laatst)   |         |
  | Gewerkt met moderne kleuren   |         |
  
  ## Wat te doen volgende week?
  Vooral de focus op de knoppen volgende week. Zorgen dat ik de default styling van alle input velden haal en mijn eigen styling hieraan meegeef. Ook moet ik nog zorgen dat er een dark en light mode komt die luistert naar de user preference.
  
</details>

<details>
  <summary>Week 4</summary>
  
  ## Voortgang
  Ik ben begonnen deze week met de knoppen van de dj mixer. Overgroot deel hiervan zijn input velden dus ik moest eerst de default styling hiervan verwijderen. Ik kwam erachter dat dit heel eenvoudig kan door middel van appearance none te gebruiken.

  Vervolgens kon ik beginnen met mijn eigen styling hieraan mee te geven. Dit was ook het moment dat ik voor het eerst gebruik ging maken van ::before en ::after. Ik ben dit al vaker tegen gekomen en dacht altijd dat dit vrij lastig is om te gebruiken maar dat valt zeker mee. Voor mij was ::before genoeg om een simpele draaiknop te maken die ik vervolgens met een animatie laat draaien.

  Ook heb ik de dark en light mode toegevoegd. Dit heb ik gedaan door middel van een mediaquery die kijkt of de gebruiker light mode heeft aan staan.

  ```
  @media (prefers-color-scheme: light) {
  :root {
    --background: var(--light-grey);
  }
  section {
    background: var(--light-grey-gradient);
  }
  section:nth-of-type(2) div:nth-of-type(1) ul li {
    background: linear-gradient(180deg, #00ff29 0%, #d0d0d0 100%);
  }
}
  ```

  Ten slotte heb ik alles nog net wat beter/mooier gemaakt door box shadows te gebruiken. Zo werd de dj set net wat realistischer en meer een geheel.

  Dit is mijn uiteindelijke uitwerking:
  <img width="1440" alt="Schermafbeelding 2023-03-09 om 12 42 10" src="https://user-images.githubusercontent.com/94384526/224049940-f085bb3e-7ed7-4658-b1ae-af58813671f7.png">

  Live te bekijken via: https://maxvl3.github.io/css-to-the-rescue-2223/

  ## Wat ging goed wat kon beter?
  | Goed      | Beter |
  | ----------- | ----------- |
  | Bijna precies aan het design wat ik had gemaakt | Ik had meer willen doen met animatie
  | Veel gedaan deze week   |         |
  | Nieuwe dingen geleerd (::before, light/dark mode)   |         |
</details>

Door: Max van Liempdt
