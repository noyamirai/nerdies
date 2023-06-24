# 3D & Three.js: Insights into WebGL and 3D Development

Servin Nissen, a full-stack developer and lead of 3D development at Level30Wizards, shared valuable insights on 3D development and the utilization of Three.js during the eight weekly nerd episode.

## WebGL and Graphics Intensive Rendering

Servin highlighted the usage of the HTML canvas element and the JavaScript-based APIs for drawing and animating graphics on the web. WebGL, an API built on OpenGL, enables the creation of graphically intensive renders on the canvas by directly communicating with the GPU. It provides the capability to create 2D and 3D graphics using shaders.

### Shaders

To work with WebGL, developers need to write shaders, which are a specialized mathematical language. There are two types of shaders: vertex shaders for defining shapes and fragment shaders for coloring the shapes. Servin mentioned the PixiJS library as a useful tool for 2D WebGL development, which closely resembles the native canvas API. Additionally, Three.js was highlighted as one of the leading 3D WebGL frameworks, simplifying the creation of WebGL-based projects.

### Optimization and Accessibility

Servin discussed the importance of optimizing 3D graphics due to their potentially heavy performance impact. Techniques such as asset compression were mentioned to improve loading times. Furthermore, accessibility considerations were emphasized, ensuring that 3D experiences are accessible to users with screen readers, keyboard navigation, and other assistive technologies. By combining HTML with the canvas element, developers can create an accessible experience for all users.

## Working with Three.js
Servin explained the fundamental components of Three.js. The axis/vector3 system in 3D development consists of X, Y, and Z axes. The scene serves as the container for rendering objects, acting as a parallel to the body tag in traditional web development. Different rendering perspectives, such as perspective and orthographic, were discussed. Lighting was also highlighted as a crucial aspect, with various types and sources of light available in 3D environments. Meshes, combining geometry and materials, represent objects in the scene, enabling the creation of complex 3D objects.

The renderer in Three.js takes the scene and camera as input and produces an image that is rendered on the canvas element. For smooth animations, the request animation frame method is utilized, ensuring a render is performed for each frame.

## Future of Web Graphics

Servin mentioned WebGPU as the successor to WebGL, providing a completely new API with modern computer graphics capabilities. WebGPU exposes technologies like Direct3D 12, Metal, and Vulkan for rendering and computation operations on the GPU. Although WebGPU is currently experimental and supported only on specific versions of Chrome (113-115), it represents the future of web graphics. Servin also mentioned WebXR, which focuses on creating websites for virtual reality (VR) and augmented reality (AR), but cautioned that support for WebXR is still limited.

## Resources

Servin shared several valuable resources for further exploration, including the ThreeJS-Journey for beginners, Simon Dev for advanced topics, and "The Book of Shaders" for in-depth understanding of fragment shaders. Servin also mentioned the abundance of open-source examples available within the Three.js community.