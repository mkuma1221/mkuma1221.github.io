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





/* ABOUT SECTION */
.about-container {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 40px;
  width: 100%;
  margin-bottom: 20px;
}

.about-text {
  width: 60%;
}

.about-skills {
  width: 40%;
}

@media (max-width: 900px) {
  .about-container {
    flex-direction: column;
  }

  .about-text,
  .about-skills {
    width: 100%;
  }
}




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

