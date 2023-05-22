# Brian | Immersive environments on the web

## Vrije tijd
vroeger lang gevoetbald
hikings!!
Houdt van lego, plantenliefhebber (bonsai), gamen

werkzaam bij Team Rockstars IT sinds april

## Social VR
vorig jaar afgestudeerd aan CMD

veel musea en organisaties moesten dicht tijdens de lockdown -> hoe connecten met ons publiek/doelgroep?

Secret Sky 2021 
online festival -> veel gebruikers kwamen samen om naar artiesten te luisteren

kwamen steeds meer van dit soort projecten uit. Social VR steeds populairder

immersive social vr in samenwerking met stedelijk museum

mogelijk om eigen character te maken, communiceren via groepscall, characters hebben verschillende expressies per thema van de kunstwerken.

## Prototypen van immersive ervaring

- Het digitale product moet aansluiten opde huidige collectie van het Stedelijk museum
 Het digitale product moet een boodschap communiceren met de gebruikers
 -Het moet een multiplayer ervaring zijn
 Gebruikers moeten communiceren
 Toegankelijk voor grote groep bezoekers
 
Starten met schetsen van plattegrond op een whiteboard (je kunt niet zo maar schermen gaan schetsen zoals bij interfaces want 3d)
maken van fysieke prototypes van karton (brown boxing)

brown boxing interactieve manier om een immersive ervaring tot leven te brengen. Simpele tools zoals karton en papier om je omgeving te bouwen. Zo snel mogelijk tot een prototype komen

hoe krijg je hier een digitale versie hiervan? lastig in figma of sketch, dus blender gebruikt als volgende stap

[snapshots van blender]

laatste stap: hoe krijg je dit op het web?

aangeven waar je mag lopen in VR met behulp van unity

ready player me -> op basis van een foto een 3d character maken (3rd party) -> ingeladen in de 3d omgeving

desktop en vr users kunnen samen in dezelfde omgeving met elkaar communiceren

## Demo time

simple plane with pills on it. one is a desktop user and the other is a VR user
VR uses teleportation for movement

alles in HTML canvas element. Tekenen van graphics. WebGL/Three.js hiermee kun je makkelijk een 3d scene maken. WebXR kan de verbinding maken met VR headset. Ondersteund ook AR

maakt gebruik van websockets om multiplayer te creeerne

WebRTC -> ook een manier om verbinding te leggen tussen andere clients (google meets gebruikt dit bijv). in de basis is het hetzelfde als websockets
UDP blijft pakketjes van data sturen ongeacht of t aankomt (normaal moet je eerst wachten tot iedereen dit pakketje ontvangt, example: gamings lag)

