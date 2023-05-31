# Triple  | Frontend setup in productie | Chanel 

Chanel is frontend developer bij Triple
houdt van games en bordspelletjes, sporten en series kijken

afgestudeerd in cmd 2018 en werkt nu bij Triple

triple okesoftware codeazure merge!!

klanten: ajax, max verstappen, citizen m, nlziet, heineken en meer!

## Webstandaarden bij Triple

Hoe ziet een gemiddelde frontend setup eruit bij Triple?

### Git

Git, gebruik je version control! Handig voor:
1. Rollback is belangrijk, je kunt altijd terug naar een oude versie in geval van nood.
2. Debugging
3. Samenwerken aan een groot en lang project

#### Werkwijze 

1. create branch vanaf main (feature branch)
2. commit & push zodra je klaar bent met feature 
3. create pull request: assign 1 of 2 andere devs voor feedback
4. code naar main. approval gehad dan mergen met main
5. deployment

### NPM
text about npm

but security risks!

- goed onderhouden/leeftijd van package
- downloads per week
- aantal contributors
- package size
- liefst zonder package dependancies
- licenses van een package checken

### Setup

Vanilla, library of framework? vanilla veel hergebruiken lol
meestal altijd een framework of library

hoe kunnen we sneller schaalbare web applicaties maken? -> overgestapt naar React/Next.js

react niet super nice voor SEO... (DOM creation)

sinds kort overgegaan naar Svelte want react breekt tv smart applicaties

Svelte is veel lichter dan react, minder code dan react, veel makkelijker op te pakken dan react, dichterbij js

### Error catching

vinden we problemen in onze code voordat ...

Typescript! (slay)

### ESLint

consistent codebase thanks to ESLint config file

### Prettier

prettier code! :D

### CSS
minder foutgevoelig?

SASS!

### Vite

snel opstarten van een project (slay)

### Livegang

React is static, nodeJS niet D: 

Azure/Azure DevOps!

Pipeline -> builden van code + validate if it works and next pipeline deploys

dev/acc/prod omgeving

dev: na pushen, development, testen
acceptatie: voor de klant
productie: productie

#### Proces
local > remote > main > dev > acc > prod

