# Servin | Level30Wizards | 3D &  Three.js

MBO > HBO > own company
Lead 3D development
Freelancer'er
Full-stack developer

Level30Wizards creative digital studio - > tech projecten en geen design (team te klein)

## 3d

With the HTML canvas element you can use Javascript to draw and animate in the web. This by using the canvas scripting API or webGL Api

WebGL is a js api with which you can create a graphicly intensive renders/drawings on the canvas element. This because the api is able to somewhat directly communicate with your gpu

WebGL is een api van het web, gemaakt op OpenGL maakt gebruik van shaders -> 2d of 3d dingen doen

openGL is een low level api

Shaders
Stel je wilt iets maken met webGL, dan moet je (helaas) shaders schrijven. Shaders is zijn eigen taal (wiskundig). Twee soorten: Vertex en fragment shaders

vertex -> shapes definieeren
fragment -> inkleuren van de shapes

PixiJS webgl library om 2d webgl mee te schrijven. een goede library om 2d dingen te doen. de api lijkt heel erg op de native canvas api

Three.js is one of the largest 3D webGL frameworks build on WebGL (dus makkelijk webgl dingen doen).

maxbox.io
kodeclubs.com
bruno-simon

Eurovision village
How to optimize 3d - 3d very heavy
Compressen van assets

Moet ook werken voor mensen met screenreader, mensen die keyboard gebruiken etc

Canvas eigenlijk gewoon een afbeelding dat re-rendered

HTML erachter gooien en het aan elkaar koppelen om zo accessible te maken

How does it work?

Axis/Vector3

in 3d heb je een 3de axis -> X, Y en Z!

Scene -> container waarin alles wordt geregenderd -> soort van body tag maar dan voor 3d
alles in scene wordt gerendered

verschillende manieren om iets te laten zien. Altijd vanuit oog van de camera: perspective en orographic

Lighting -> binnen 3d als je je lichtbron vergeet zie je alleen maar zwart. (er zijn verschillende soorten en typen lichtbronnen die je kunt gebruiken)

Meshes -> basically geef je hiermee een object echt in de wereld. T heeft een geometry (box bijv) en dan een material. als jje deze twee combineerd met een mesh dan heb je een box in een scene

Renderer pakt je scene en je camera -> maakt een afbeelding en zet dit in je canvas element

Met motion -> request animation frame met elke mogelijke frame een render maken.

## Future*

WebGPU opvolger van webGl voledig nieuwe api.

Webgpu is a new web api that exposes modern computer graphcis capabilities. specifically direct3d 12, metal, and vulkan, for performing rendering and computation operations on a GPU

WebGPU barely supported / very experimental (only on chrome 113 - 115)

WebXR -> websites for vr and ar maken (barely supported)

Resources:

ThreeJS-Journey (beginner)
Simon Dev (advanced)
The book of shaders (huilen fragment shaders)
Three.js heeft tering veel examples open source