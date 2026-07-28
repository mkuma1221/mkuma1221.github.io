<style>
  /* GLOBAL TYPOGRAPHY */
  body, .main-content {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif !important;
    color: #334155;
    line-height: 1.65;
  }

  .page-header {
    background-image: url('images/GAX.jpg') !important;
    background-size: cover !important;
    background-position: center !important;
  }

  /* PROJECT IMAGES */
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

  /* DIVIDER */
  .project-divider {
    width: 100%;
    height: 1px;
    background-color: #E2E8F0;
    margin: 16px 0 24px 0;
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

  /* SECTION HEADINGS */
  .section-title {
    color: #1B365D;
    font-size: 1.75rem;
    font-weight: 700;
    letter-spacing: -0.02em;
    margin-top: 20px;
    margin-bottom: 12px;
  }

  /* PROJECT TITLE */
  .project-title {
    color: #1B365D;
    font-size: 1.35rem;
    font-weight: 600;
    margin-bottom: 12px;
    text-align: center;
    letter-spacing: -0.01em;
  }

  /* GHOST BUTTON */
  .project-button {
    display: inline-block;
    margin-top: 10px;
    padding: 10px 18px;
    border: 2px solid #007bff;
    border-radius: 8px;
    color: #007bff;
    text-decoration: none !important;
    font-weight: 600;
    font-size: 0.95rem;
    transition: background-color 0.2s ease,
                color 0.2s ease,
                transform 0.2s ease,
                box-shadow 0.2s ease;
  }

  .project-button:hover {
    background-color: #007bff;
    color: white;
    text-decoration: none !important;
    transform: translateY(-2px);
    box-shadow: 0 4px 10px rgba(0, 123, 255, 0.2);
  }

  /* PROJECT BULLETS */
  .project-text ul {
    list-style-type: square;
    padding-left: 22px;
    color: #475569;
  }

  .project-text li {
    margin-bottom: 8px;
  }

  /* SKILL GROUPS */
  .skill-group {
    margin-bottom: 18px;
  }

  .skill-group h3 {
    margin-bottom: 8px;
    color: #475569;
    font-size: 1rem;
    font-weight: 600;
  }

  /* SKILL PILL CONTAINER */
  .skill-pills {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  /* INDIVIDUAL SKILL PILLS */
  .skill-pill {
    display: inline-block;
    padding: 4px 12px;
    background-color: #F8FAFC;
    border: 1px solid #E2E8F0;
    border-radius: 14px;
    font-size: 0.85em;
    font-weight: 500;
    color: #334155;
    line-height: 1.3;
    transition: background-color 0.2s ease,
                transform 0.2s ease,
                box-shadow 0.2s ease;
  }

  .skill-pill:hover {
    background-color: #E0F2FE;
    border-color: #BAE6FD;
    transform: translateY(-1px);
    box-shadow: 0 2px 6px rgba(0,0,0,0.06);
  }
</style>

<table style="width:100%; border-collapse:collapse; border:none; margin-bottom:20px;">
  <tr>
    <td style="width:60%; vertical-align:top; padding-right:35px; border:none;">
      <h2 class="section-title">About Me</h2>
      <p style="color:#334155; margin-bottom:0;">
        Hi, my name is Mohana Kumanan, and I am an aerospace engineering student with an interest in control systems and orbital mechanics. I have experience in technical analysis, collaborative engineering projects, MATLAB, Simulink, numerical methods, and spacecraft dynamics. This website serves as a technical portfolio documenting the engineering methodologies, analyses, and computational tools developed throughout my projects.
      </p>
    </td>

    <td style="width:40%; vertical-align:top; border:none;">
      <h2 class="section-title">Technical Skills</h2>

      <div class="skill-group">
        <h3>Programming</h3>
        <div class="skill-pills">
          <span class="skill-pill">MATLAB</span>
          <span class="skill-pill">Python</span>
          <span class="skill-pill">C++</span>
        </div>
      </div>

      <div class="skill-group">
        <h3>Software</h3>
        <div class="skill-pills">
          <span class="skill-pill">Simulink</span>
          <span class="skill-pill">Stateflow</span>
          <span class="skill-pill">SolidWorks</span>
          <span class="skill-pill">Ansys</span>
          <span class="skill-pill">FlightGear</span>
          <span class="skill-pill">STAR-CCM+</span>
          <span class="skill-pill">Altium</span>
        </div>
      </div>
    </td>
  </tr>
</table>

<h2 class="section-title">Projects</h2>
<div class="project-divider"></div>

<h3 class="project-title">
  Kepler’s Problem Solver & Orbital Propagation
</h3>

<div class="project-container">
  <div class="project-text">
    <ul>
      <li>Solved Kepler's equation using the Newton–Raphson iterative method.</li>
      <li>Computed Classical Orbital Elements (COEs).</li>
      <li>Verified conservation of orbital energy and angular momentum.</li>
      <li>Transformed states between perifocal and ECI reference frames.</li>
    </ul>

    <a href="kepler-solver.html" class="project-button">View More Details</a>
  </div>

  <div class="project-media">
    <img src="images/SAT.png" alt="Satellite Trajectory" style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto;">
    <p style="font-size: 0.85em; color: #64748B; margin-top: 6px; font-style: italic;">
      Comparison of Newton-Raphson to ODE45
    </p>
  </div>
</div>

<div class="project-divider"></div>

<h3 class="project-title">
  Pitch Autopilot Controller Model
</h3>

<div class="project-container">
  <div class="project-text">
    <ul>
      <li>Designed a PID controller with anti-windup and actuator dynamics.</li>
      <li>Implemented Kalman filtering for robust state estimation.</li>
      <li>Evaluated controller performance using step, doublet, and square-wave reference inputs.</li>
      <li>Visualized aircraft response through real-time FlightGear 6DOF simulation.</li>
    </ul>

    <a href="pitch-controller.html" class="project-button">View More Details</a>
  </div>

  <div class="project-media">
    <img src="images/cessna.png" alt="Closed-Loop Pitch Controller" style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto;">
    <p style="font-size: 0.85em; color: #64748B; margin-top: 6px; font-style: italic;">
      Closed-Loop Pitch Controller in Action
    </p>
  </div>
</div>

