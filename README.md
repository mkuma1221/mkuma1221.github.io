<style>
  .page-header {
    background-image: url('GAX.jpg') !important;
    background-size: cover !important;
    background-position: center !important;
  }
  

  /* PROJECT IMAGES (ADDED NEW) */
.project-media img {
  border-radius: 10px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.12);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
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

  
  .main-content {
  max-width: 1400px !important;
  width: 92% !important;
  margin: 0 auto !important;
}

  
/* GHOST BUTTON */ .project-button { 
  display: inline-block; 
  margin-top: 8px; 
  padding: 10px 18px; 
  border: 2px solid #007bff; 
  border-radius: 8px; color: #007bff; 
  text-decoration: none; 
  font-family: sans-serif; 
  font-weight: 600; transition: background-color 0.2s ease, 
                                color 0.2s ease, 
                                transform 0.2s ease, 
                                box-shadow 0.2s ease; 

}
.project-button:hover { 
  background-color: #007bff; 
  color: white; 
  transform: translateY(-2px); 
  box-shadow: 0 4px 10px rgba(0, 123, 255, 0.2);
}

/* PROJECT BULLETS */
.project-text ul {
  list-style-type: square;
  padding-left: 22px;
}

.project-text li {
  margin-bottom: 6px;
}
  
</style>





<!-- ABOUT ME SECTION AND SKILLS -->


<table style="width:100%; border-collapse:collapse; border:none; margin-bottom:20px;">
  <tr>

    <!-- LEFT COLUMN (60%) -->
    <td style="width:60%; vertical-align:top; padding-right:35px; border:none;">

      <h2 style="color:#000080; font-size:1.8em; margin-top:20px; margin-bottom:10px; font-family:sans-serif;">
        About Me
      </h2>

      <p style="color:#444; line-height:1.6; font-family:sans-serif; margin-bottom:0;">
        Hi, my name is Mohana Kumanan, and I am an aerospace engineering student with a focus on control systems and orbital mechanics. I have experience in technical analysis, collaborative engineering projects, MATLAB, Simulink, numerical methods, and spacecraft dynamics. This website serves as a technical portfolio documenting the engineering methodologies, analyses, and computational tools developed throughout my projects.
      </p>

    </td>

    <!-- RIGHT COLUMN (40%) -->
    <td style="width:40%; vertical-align:top; border:none;">

      <h2 style="color:#000080; font-size:1.8em; margin-top:20px; margin-bottom:10px; font-family:sans-serif;">
        Technical Skills
      </h2>

      <p style="margin-bottom:6px;"><strong>Programming</strong></p>
      <p style="margin-top:0; color:#444;">
        MATLAB • Python • C++
      </p>

      <p style="margin-bottom:6px;"><strong>Software</strong></p>
      <p style="margin-top:0; color:#444;">
        Simulink • Stateflow • Solidworks • Ansys • FlightGear • STAR-CCM+ • Altium
      </p>

     

    </td>

  </tr>
</table>







<!--     PROJECTS       SECTION  -->


<h2 style="color: #000080; font-size: 1.8em; margin-bottom: 6px; font-family: sans-serif;">
  Projects
</h2>

<div class="project-divider"></div>

<h3 style="color: #000080; font-size: 1.4em; margin-bottom: 10px; text-align: center; font-family: sans-serif;">
  Kepler’s Problem Solver & Orbital Propagation
</h3>

<div class="project-container">

  <div class="project-text">

    <ul style="color:#444; line-height:1.6; margin-top:6px; margin-bottom:12px; padding-left:20px; font-family:sans-serif;">
    <li>Solved Kepler's equation using the Newton–Raphson iterative method.</li>
    <li>Computed Classical Orbital Elements (COEs).</li>
    <li>Verified conservation of orbital energy and angular momentum.</li>
    <li>Transformed states between perifocal and ECI reference frames.</li>
    </ul>

<a href="kepler-solver.html" class="project-button">
  View More Details
</a>

  </div>

  <div class="project-media">

    <img src="SAT.png"
     alt="Satellite Trajectory"
     style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto;">

         <p style="font-size: 0.85em; color: #666; margin-top: 6px; font-family: sans-serif; font-style: italic;">
      Comparison of Newton-Raphson to ODE45
    </p>
    
  </div>

</div>

<div class="project-divider"></div>

<h3 style="color: #000080; font-size: 1.4em; margin-bottom: 10px; text-align: center; font-family: sans-serif;">
  Pitch Autopilot Controller Model
</h3>

<div class="project-container">

  <div class="project-text">

    <ul style="color:#444; line-height:1.6; margin-top:6px; margin-bottom:12px; font-family:sans-serif;">
    <li>Designed a PID controller with anti-windup and actuator dynamics.</li>
    <li>Implemented Kalman filtering for robust state estimation.</li>
    <li>Evaluated controller performance using step, doublet, and square-wave reference inputs.</li>
    <li>Visualized aircraft response through real-time FlightGear 6DOF simulation.</li>
    </ul>

<a href="kepler-solver.html" class="project-button">
  View More Details
</a>
  </div>

  <div class="project-media">

     <img src="cessna.png"
     alt="Closed-Loop Pitch Controller"
     style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto;">

    <p style="font-size: 0.85em; color: #666; margin-top: 6px; font-family: sans-serif; font-style: italic;">
    Closed-Loop Pitch Controller in Action
    </p>

  </div>

</div>



