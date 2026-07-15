<style>
  .page-header {
    background-image: url('GAX.jpg') !important;
    background-size: cover !important;
    background-position: center !important;
  }

  /* Make page wider */
  .main-content {
    max-width: 1400px !important;
    width: 92% !important;
    margin: 0 auto !important;
  }

  /* PROJECT LAYOUT */
  .project-container {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    align-items: flex-start;
    border: none !important;
    margin-top: 6px;
    margin-bottom: 6px;
  }

  

  .page-header {
    background-image: url('GAX.jpg') !important;
    background-size: cover !important;
    background-position: center !important;
  }

  /* PROJECT LAYOUT */
  .project-container {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    align-items: flex-start;
    border: none !important;
    margin-top: 6px;
    margin-bottom: 6px;
  }

  .project-text {
    flex: 1 1 50%;
    min-width: 300px;
    border: none !important;
  }

  .project-media {
    flex: 1 1 40%;
    min-width: 300px;
    text-align: center;
    border: none !important;
  }

  /* DIVIDER (slightly bolder + tight spacing) */
  .project-divider {
    width: 100%;
    height: 2px;
    background-color: #bfbfbf;
    margin: 8px 0;
  }

  /* REMOVE EXTRA DEFAULT SPACING */
  h2, h3, p {
    margin-top: 0;
  }

  img, div, section {
    border: none !important;
  }
</style>

<h2 style="color: #000080; font-size: 1.8em; margin-top: 20px; margin-bottom: 10px; font-family: sans-serif;">
  About Me
</h2>

<p style="color: #444; line-height: 1.6; font-family: sans-serif; margin-bottom: 18px;">
  Hi, my name is Mohana Kumanan, and I am an aerospace engineering student with a focus on control systems and orbital mechanics. I have experience in both technical analysis and collaborative engineering projects, with a strong interest in applying aerospace engineering principles to real-world systems. Through my coursework and projects, I have developed a solid foundation in orbital mechanics, dynamics, and control systems, along with practical experience in MATLAB, numerical methods, system modeling, and spacecraft state propagation. These experiences have strengthened my ability to analyze complex engineering problems, develop computational solutions, and validate results through analytical and numerical techniques. This website serves as both a technical portfolio and a professional archive, documenting the methodologies, analysis, and engineering concepts developed throughout my projects while showcasing the technical experience and skills I have gained.
</p>

<h2 style="color: #000080; font-size: 1.8em; margin-bottom: 6px; font-family: sans-serif;">
  Projects
</h2>

<div class="project-divider"></div>

<h3 style="color: #000080; font-size: 1.4em; margin-bottom: 10px; text-align: center; font-family: sans-serif;">
  Kepler’s Problem Solver & Orbital Propagation
</h3>

<div class="project-container">

  <div class="project-text">

    <p style="color: #444; line-height: 1.6; margin-bottom: 8px; font-family: sans-serif;">
      Developed a MATLAB orbital mechanics simulation to solve Kepler’s equation using the Newton–Raphson iterative method. The project computed Classical Orbital Elements from given position, velocity, and gravitational parameter, verified results through conservation of orbital energy and angular momentum, and used Direction Cosine Matrices to transform states between perifocal and ECI reference frames.
    </p>

<a href="kepler-solver.html"
   style="font-family: sans-serif; text-decoration: none; color: #007bff; font-weight: bold;">
  View More Details
</a>

  </div>

  <div class="project-media">

    <img src="SAT.png"
         alt="Satellite Trajectory"
         style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto; border-radius: 4px;">

    <p style="font-size: 0.85em; color: #666; margin-top: 6px; font-family: sans-serif; font-style: italic;">
      Comparison of Newton–Raphson to ODE45
    </p>

  </div>

</div>

<div class="project-divider"></div>












<h3 style="color: #000080; font-size: 1.4em; margin-bottom: 10px; text-align: center; font-family: sans-serif;">
  Pitch Autopilot Controller Model
</h3>

<div class="project-container">

  <div class="project-text">

    <p style="color: #444; line-height: 1.6; margin-bottom: 8px; font-family: sans-serif;">
  Developed a closed-loop pitch autopilot in Simulink and validated its performance through real-time integration with the FlightGear flight simulator. The project implemented a PID controller with anti-windup, actuator dynamics, simulated aerodynamic disturbances, and Kalman filtering for robust state estimation, and evaluated controller performance using step, doublet, and square-wave reference inputs while visualizing the aircraft's 6-Degrees-of-Freedom (6DOF) response in a real-time 3D flight environment.
    </p>

<a href="kepler-solver.html"
   style="font-family: sans-serif; text-decoration: none; color: #007bff; font-weight: bold;">
  View More Details
</a>

  </div>

  <div class="project-media">

    <img src="cessna.png"
         alt="Satellite Trajectory"
         style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto; border-radius: 4px;">

    <p style="font-size: 0.85em; color: #666; margin-top: 6px; font-family: sans-serif; font-style: italic;">
     Closed-Loop Pitch Controller in Action   
    </p>

  </div>

</div>

<div class="project-divider"></div>

