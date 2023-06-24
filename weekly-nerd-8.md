# Immersive Environments on the Web: Connecting Audiences through Social VR

Brian, a developer at Team Rockstars IT and recent graduate of CMD, discussed the concept of immersive environments on the web, focusing on Social VR and its applications in connecting museums and organizations with their audiences.

## Background and Social VR

Brian shared his interest in hobbies such as football, hiking, Lego, plants (bonsai), and gaming. He highlighted the need for museums and organizations to connect with their audiences during the lockdown period. Brian mentioned the Secret Sky 2021 online festival, where users gathered virtually to listen to artists, as an example of the growing popularity of Social VR. He also discussed a collaboration with the Stedelijk Museum to create an immersive Social VR experience, allowing users to create their own characters, communicate via group calls, and express different emotions based on the artwork themes.

## Prototyping for the collab with Stedelijk Museum

To prototype an immersive Social VR experience, Brian outlined several key considerations:

- The digital product should align with the Stedelijk Museum's current collection.
- The digital product should effectively communicate a message to the users.
- It should be a multiplayer experience, encouraging user interaction.
- Accessibility should be a priority to accommodate a large group of visitors.

Brian explained the prototyping process, starting with sketching the floor plan on a whiteboard. As interfaces are not two-dimensional, physical prototypes made of cardboard (brown boxing) were used to bring the immersive experience to life quickly. Blender, a 3D modeling software, was then employed to create a digital version of the prototypes.

## Bringing the Experience to the Web

Brian addressed the challenge of bringing the immersive experience to the web. Unity was used to indicate user movement paths in VR. Ready Player Me, a third-party tool, allowed the creation of 3D characters based on user photos, which were then integrated into the 3D environment. Desktop and VR users could interact and communicate within the same environment.

### Demo and Technical Aspects

During the demo of the Social VR experience he created, Brian showcased a simple plane with pills on it, with one user in desktop mode and another in VR mode. The VR user utilized teleportation for movement. 

Brian explained that the entire experience was built using HTML canvas elements for graphics rendering. WebGL and Three.js were utilized to create the 3D scene, while WebXR facilitated the connection with VR headsets and also supported augmented reality (AR). Brian mentioned the use of websockets for multiplayer functionality and highlighted WebRTC as an alternative for establishing connections between clients, similar to how Google Meet utilizes it.

He explained that WebRTC operates on UDP, allowing continuous data packet transmission regardless of whether each packet is received instantly (as opposed to waiting for all packets to arrive, which can cause lag in gaming scenarios).
