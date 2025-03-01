Create a p5.js simulation of a floating light maroon satin handkerchief with the following specifications:

VISUAL REQUIREMENTS:
- The handkerchief should be a single, continuous piece of cloth (not separate strips)
- Use a 30x30 grid of particles for a high-resolution cloth mesh
- Light maroon color with satin-like material properties (specular highlights)
- Directional lighting from a 60-degree angle in all three dimensions (x, y, z)
- Additional fill light to enhance the 3D appearance
- Pixel density of 2 for higher visual quality

PHYSICS REQUIREMENTS:
- Verlet integration for cloth physics
- A gentle constant breeze effect that causes the handkerchief to float
- Constraint-based system for maintaining cloth structure
- A restore force that returns the cloth to its original shape
- Adaptive time stepping based on frame rate for stability

INTERACTION:
- Mouse clicks should disturb the cloth, creating ripples
- The handkerchief should gently restore back to its floating state after disturbance

DEBUG FEATURES:
- Include a debug panel with the following controls:
  - Toggle Debug View button (shows wireframe, forces, and constraint stress)
  - Reset Cloth button
  - Sliders for Breeze Strength, Restore Force, Damping, Light Angle, and Pixel Density
  - FPS counter and particle information display

IMPLEMENTATION DETAILS:
- Use TRIANGLES for drawing the cloth (not TRIANGLE_STRIP) to ensure a continuous surface
- Include additional structural constraints between non-adjacent vertices for stability
- Calculate proper surface normals for realistic lighting
- Use smooth camera movement to better showcase the 3D effect
- The cloth should float in the center of the screen

The final result should run smoothly in a web browser and look like a realistic piece of satin cloth floating in the air.