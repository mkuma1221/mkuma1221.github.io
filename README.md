<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet">

<style>
  /* GLOBAL FONT & HEADER COLOR CONFIGURATION */
  body, p, li, a, span, button {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif !important;
  }

  /* Modern Headings Style & Color */
  h1, h2, h3, h4 {
    font-family: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif !important;
    color: #1e293b !important; /* Deep Slate Blue/Charcoal (replaces navy) */
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
    height: 2px;
    background-color: #e2e8f0;
    margin: 12px 0;
  }

  /* SPACING & TYPOGRAPHY */
  h2, h3, p {
    margin-top: 0;
  }

  h2 {
    font-weight: 700;
    letter-spacing: -0.025em;
  }

  h3 {
    font-weight: 600;
    letter-spacing: -0.015em;
  }

  img, div, section {
    border: none !important;
  }

  .main-content {
    max-width: 1400px !important;
    width: 92% !important;
    margin: 0 auto !important;
  }

  /* GHOST BUTTON */
  .project-button {
    display: inline-block;
    margin-top: 8px;
    padding: 10px 18px;
    border: 2px solid #2563eb;
    border-radius: 8px;
    color: #2563eb;
    text-decoration: none !important;
    font-weight: 600;
    font-size: 0.9em;
    transition: background-color 0.2s ease,
                color 0.2s ease,
                transform 0.2s ease,
                box-shadow 0.2s ease;
  }

  .project-button:hover {
    background-color: #2563eb;
    color: white;
    text-decoration: none !important;
    transform: translateY(-2px);
    box-shadow: 0 4px 10px rgba(37, 99, 235, 0.2);
  }

  /* PROJECT BULLETS */
  .project-text ul {
    list-style-type: square;
    padding-left: 22px;
  }

  .project-text li {
    margin-bottom: 6px;
  }

  /* SKILL GROUPS */
  .skill-group {
    margin-bottom: 18px;
  }

  .skill-group h3 {
    margin-bottom: 8px;
    color: #475569;
    font-size: 1.05em;
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
    padding: 5px 12px;
    background-color: #f8fafc;
    border: 1px solid #cbd5e1;
    border-radius: 14px;
    font-size: 0.85em;
    font-weight: 500;
    color: #334155;
    line-height: 1.2;
    transition: all 0.3s ease;
    cursor: pointer;
  }

  /* Hover glow animation (lasts 1.5 seconds then fades away) */
  .skill-pill:hover {
    animation: temporaryGlow 1.5s ease-out forwards;
  }

  @keyframes temporaryGlow {
    0% {
      background-color: #ffffff;
      border-color: var(--glow-color);
      box-shadow: 0 0 10px var(--glow-color);
      transform: translateY(-2px);
      color: var(--glow-color);
      font-weight: 600;
    }
    60% {
      background-color: #ffffff;
      border-color: var(--glow-color);
      box-shadow: 0 0 10px var(--glow-color);
      transform: translateY(-2px);
      color: var(--glow-color);
      font-weight: 600;
    }
    100% {
      background-color: #f8fafc;
      border-color: #cbd5e1;
      box-shadow: none;
      transform: translateY(0);
      color: #334155;
      font-weight: 500;
    }
  }

  /* Brand-Specific Glow Colors */
  .skill-pill.matlab     { --glow-color: #e05206; } /* MATLAB Orange */
  .skill-pill.python     { --glow-color: #306998; } /* Python Blue */
  .skill-pill.cpp        { --glow-color: #00599c; } /* C++ Dark Blue */
  .skill-pill.simulink   { --glow-color: #0076a8; } /* Simulink Blue */
  .skill-pill.stateflow  { --glow-color: #008080; } /* Stateflow Teal */
  .skill-pill.solidworks { --glow-color: #d12727; } /* SolidWorks Red */
  .skill-pill.ansys      { --glow-color: #e6a100; } /* Ansys Gold */
  .skill-pill.flightgear { --glow-color: #009999; } /* FlightGear Teal */
  .skill-pill.starccm    { --glow-color: #00a3a6; } /* Siemens Teal */
  .skill-pill.altium     { --glow-color: #cc9900; } /* Altium Gold */
</style>

<table style="width:100%; border-collapse:collapse; border:none; margin-bottom:20px;">
  <tr>
    <td style="width:60%; vertical-align:top; padding-right:35px; border:none;">
      <h2 style="font-size:1.8em; margin-top:20px; margin-bottom:10px;">
        About Me
      </h2>
      <p style="color:#475569; line-height:1.6; margin-bottom:0;">
        Hi, my name is Mohana Kumanan, and I am an aerospace engineering student with an interest in control systems and orbital mechanics. I have experience in technical analysis, collaborative engineering projects, MATLAB, Simulink, numerical methods, and spacecraft dynamics. This website serves as a technical portfolio documenting the engineering methodologies, analyses, and computational tools developed throughout my projects.
      </p>
    </td>

    <td style="width:40%; vertical-align:top; border:none;">
      <h2 style="font-size:1.8em; margin-top:20px; margin-bottom:18px;">
        Technical Skills
      </h2>

      <div class="skill-group">
        <h3>Programming</h3>
        <div class="skill-pills">
          <span class="skill-pill matlab">MATLAB</span>
          <span class="skill-pill python">Python</span>
          <span class="skill-pill cpp">C++</span>
        </div>
      </div>

      <div class="skill-group">
        <h3>Software</h3>
        <div class="skill-pills">
          <span class="skill-pill simulink">Simulink</span>
          <span class="skill-pill stateflow">Stateflow</span>
          <span class="skill-pill solidworks">SolidWorks</span>
          <span class="skill-pill ansys">Ansys</span>
          <span class="skill-pill flightgear">FlightGear</span>
          <span class="skill-pill starccm">STAR-CCM+</span>
          <span class="skill-pill altium">Altium</span>
        </div>
      </div>
    </td>
  </tr>
</table>

<h2 style="font-size: 1.8em; margin-bottom: 6px;">
  Projects
</h2>

<div class="project-divider"></div>

<h3 style="font-size: 1.4em; margin-bottom: 10px; text-align: center;">
  Kepler’s Problem Solver & Orbital Propagation
</h3>

<div class="project-container">
  <div class="project-text">
    <ul style="color:#475569; line-height:1.6; margin-top:6px; margin-bottom:12px; padding-left:20px;">
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
    <img src="images/SAT.png"
         alt="Satellite Trajectory"
         style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto;">
    <p style="font-size: 0.85em; color: #64748b; margin-top: 6px; font-style: italic;">
      Comparison of Newton-Raphson to ODE45
    </p>
  </div>
</div>

<div class="project-divider"></div>

<h3 style="font-size: 1.4em; margin-bottom: 10px; text-align: center;">
  Pitch Autopilot Controller Model
</h3>

<div class="project-container">
  <div class="project-text">
    <ul style="color:#475569; line-height:1.6; margin-top:6px; margin-bottom:12px;">
      <li>Designed a PID controller with anti-windup and actuator dynamics.</li>
      <li>Implemented Kalman filtering for robust state estimation.</li>
      <li>Evaluated controller performance using step, doublet, and square-wave reference inputs.</li>
      <li>Visualized aircraft response through real-time FlightGear 6DOF simulation.</li>
    </ul>

    <a href="pitch-controller.html" class="project-button">
      View More Details
    </a>
  </div>

  <div class="project-media">
    <img src="images/cessna.png"
         alt="Closed-Loop Pitch Controller"
         style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto;">
    <p style="font-size: 0.85em; color: #64748b; margin-top: 6px; font-style: italic;">
      Closed-Loop Pitch Controller in Action
    </p>
  </div>
</div>
