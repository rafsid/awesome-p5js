Here's a prompt that describes the fluid simulation I created:
"Create an interactive fluid dynamics simulation using P5.js wrapped in HTML. Implement Jos Stam's fluid solver algorithm that simulates the Navier-Stokes equations. The simulation should:

Allow users to interact by clicking and dragging to add velocity and density to the fluid
Include proper physics for diffusion, advection, and pressure solving
Feature colorful visualization that changes over time (with at least 3 different color modes that can be toggled with the 'c' key)
Have a reset function (triggered by the 'r' key)
Be responsive to window size
Include a semi-transparent background for beautiful trailing effects
Display small instruction text for user guidance

The grid resolution should be 64x64 cells, with appropriate viscosity and diffusion parameters for smooth, realistic fluid behavior. Ensure the code is well-commented to explain the core simulation functions including the velocity step, density step, diffusion, advection, and projection operations.