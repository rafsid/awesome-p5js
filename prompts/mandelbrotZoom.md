Create a Mandelbrot set explorer using p5.js that allows smooth, interactive exploration of the fractal. The application should have the following
  features:

  1. Core visualization:
     - Render the Mandelbrot set with customizable maximum iterations
     - Support zooming to arbitrary depths with proper precision
     - Use smooth coloring to eliminate banding artifacts
     - Display the current coordinates, zoom level, and render time

  2. Performance optimizations:
     - Use double buffers for rendering - a high-quality buffer for static views, and a low-res buffer for interactions
     - Implement pixel sampling during interactive operations
     - Add early escape optimizations for the main cardioid and period-2 bulb
     - Use cached calculations for improved performance
     - Implement smooth color transitions between iteration bands

  3. Interactive features:
     - Left-click to zoom in at cursor position
     - Right-click to zoom out at cursor position
     - Click and drag to pan around
     - Smooth zoom animations with easing
     - A "gravity zoom" feature that accelerates zoom based on physics (d = 0.5*g*t²)

  4. UI controls:
     - Slider to adjust maximum iteration count (50-10000)
     - Slider to adjust zoom speed
     - Dropdown to select different color schemes (rainbow, fire, ocean, grayscale, electric)
     - Reset button to return to default view
     - Save button to export current view as PNG
     - Toggle button for gravity zoom

  5. Color schemes:
     - Rainbow: Cycling hues based on iteration count
     - Fire: Red to yellow to white gradient
     - Ocean: Deep blue to cyan to white gradient
     - Grayscale: Black to white gradient
     - Electric: Purple-blue gradient

  Ensure that dragging preserves colors (no recalculation during dragging) and that the UI is clean and minimalistic. Add performance optimizations
  like debounced rendering and smart buffer management to maintain smooth framerates even at high iteration counts.