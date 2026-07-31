<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet">

<style>
  /* GLOBAL FONT OVERRIDES */
  body, p, li, a, span, button, td, div {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif !important;
    color: #334155;
    line-height: 1.55;
  }

  /* Specific targeting for About Me text */
  .about-text, .about-text p {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif !important;
    color: #334155 !important;
    font-size: 0.95em !important;
    line-height: 1.6 !important;
  }

  /* Modern Headings Style & Color */
  h1, h2, h3, h4 {
    font-family: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif !important;
    color: #1e293b !important;
    font-weight: 700 !important;
  }

  .page-header {
    background-image: url('images/GAX.jpg') !important;
    background-size: cover !important;
    background-position: center !important;
  }

  /* --- FLEX LAYOUT FOR ABOUT ME & SKILLS (Replaces <table>) --- */
  .about-skills-container {
    display: flex;
    flex-wrap: wrap;
    gap: 35px;
    margin-bottom: 30px;
  }

  .about-column {
    flex: 1 1 55%; /* Takes ~60% on desktop */
  }

  .skills-column {
    flex: 1 1 35%; /* Takes ~40% on desktop */
  }

  /* --- SLIGHTLY LARGER GRID LAYOUT FOR PROJECTS --- */
  .projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
    margin-top: 14px;
    margin-bottom: 28px;
  }

  /* SHADED CARDS (STATIONARY - NO HOVER MOVEMENT) */
  .project-card {
    background-color: #f8fafc;
    border: 1px solid #e2e8f0 !important;
    border-radius: 12px;
    padding: 16px;
    box-shadow: 0 1px 4px rgba(0, 0, 0, 0.05);
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  /* FULL IMAGE SHOWCASE (NO CUTOFF / FULL SIZE) */
  .project-media {
    text-align: center;
    border: none !important;
    margin-bottom: 10px;
  }

  .project-media img {
    width: 100%;
    height: auto;
    max-height: 200px;
    object-fit: contain;
    border-radius: 8px;
    display: block;
    margin: 0 auto;
    box-shadow: 0 1px 4px rgba(0, 0, 0, 0.08);
  }

  .project-text {
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    border: none !important;
  }

  .project-card h3 {
    font-size: 1.1em !important;
    margin-bottom: 8px;
    line-height: 1.35;
    text-align: left;
  }

  /* SPACING & CLEANUP */
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

  /* BUTTON STYLING */
  .project-button {
    display: inline-block;
    align-self: flex-start;
    margin-top: 10px;
    padding: 7px 14px;
    border: 1.5px solid #2563eb;
    border-radius: 6px;
    color: #2563eb !important;
    text-decoration: none !important;
    font-weight: 600 !important;
    font-size: 0.85em;
    transition: background-color 0.2s ease, color 0.2s ease;
  }

  .project-button:hover {
    background-color: #2563eb;
    color: #ffffff !important;
    text-decoration: none !important;
  }

  /* PROJECT BULLETS */
  .project-text ul {
    list-style-type: square;
    padding-left: 18px;
    margin-top: 4px;
    margin-bottom: 8px;
  }

  .project-text li {
    margin-bottom: 5px;
    font-size: 0.85em;
    color: #475569 !important;
    line-height: 1.4;
  }

  /* SKILL GROUPS */
  .skill-group {
    margin-bottom: 18px;
  }

  .skill-group h3 {
    margin-bottom: 8px;
    color: #475569 !important;
    font-size: 1.05em;
    font-weight: 600 !important;
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
    font-weight: 500 !important;
    color: #334155 !important;
    line-height: 1.2;
    transition: all 0.3s ease;
    cursor: pointer;
  }

  .skill-pill:hover {
    animation: temporaryGlow 1.5s ease-out forwards;
  }

  @keyframes temporaryGlow {
    0% {
      background-color: #ffffff;
      border-color: var(--glow-color);
      box-shadow: 0 0 10px var(--glow-color);
      transform: translateY(-2px);
      color: var(--glow-color) !important;
      font-weight: 600 !important;
    }
    60% {
      background-color: #ffffff;
      border-color: var(--glow-color);
      box-shadow: 0 0 10px var(--glow-color);
      transform: translateY(-2px);
      color: var(--glow-color) !important;
      font-weight: 600 !important;
    }
    100% {
      background-color: #f8fafc;
      border-color: #cbd5e1;
      box-shadow: none;
      transform: translateY(0);
      color: #334155 !important;
      font-weight: 500 !important;
    }
  }

  /* Brand-Specific Glow Colors */
  .skill-pill.matlab     { --glow-color: #e05206; }
  .skill-pill.python     { --glow-color: #306998; }
  .skill-pill.cpp        { --glow-color: #00599c; }
  .skill-pill.simulink   { --glow-color: #0076a8; }
  .skill-pill.stateflow  { --glow-color: #008080; }
  .skill-pill.solidworks { --glow-color: #d12727; }
  .skill-pill.ansys      { --glow-color: #e6a100; }
  .skill-pill.flightgear { --glow-color: #009999; }
  .skill-pill.starccm    { --glow-color: #00a3a6; }
  .skill-pill.altium     { --glow-color: #cc9900; }

  /* --- MOBILE SPECIFIC STYLES --- */
  @media screen and (max-width: 768px) {
    .about-skills-container {
      flex-direction: column; /* Stacks About Me on top of Skills on phones */
      gap: 10px;
    }

    .about-column, .skills-column {
      flex: 1 1 100%;
      width: 100%;
    }

    .projects-grid {
      grid-template-columns: 1fr; /* Stacks project cards into 1 column */
    }

    .main-content {
      width: 95% !important;
      padding: 10px !important;
    }
  }
</style>

<div class="about-skills-container">
  <div class="about-column about-text">
    <h2 style="font-size:1.8em; margin-top:20px; margin-bottom:12px;">
      About Me
    </h2>
    <p style="margin-bottom:0;">
      Hi, I'm Mohana Kumanan, an aerospace engineering student with a primary focus on Guidance, Navigation, and Control (GNC), orbital mechanics, and aerospace structures. My experience centers on technical analysis, spacecraft dynamics, and computational modeling. I regularly use MATLAB, Simulink, and numerical methods to model, analyze, and validate complex aerospace systems. This portfolio showcases the computational tools, engineering methodologies, and technical projects I have developed throughout my academic and personal work. This portfolio will continue to grow as I complete new projects. If you have any feedback or would like to connect, please feel free to reach out.
    </p>
  </div>

  <div class="skills-column">
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
  </div>
</div>

<h2 style="font-size: 1.8em; margin-bottom: 12px;">
  Projects
</h2>

<div class="projects-grid">

  <div class="project-card">
    <div class="project-media">
      <img src="images/SAT.png" alt="Satellite Trajectory">
      <p style="font-size: 0.78em; color: #64748b !important; margin-top: 5px; font-style: italic; margin-bottom: 0;">
        Comparison of Newton-Raphson to ODE45
      </p>
    </div>

    <div class="project-text">
      <div>
        <h3>Kepler’s Problem Solver & Orbital Propagation</h3>
        <ul>
          <li>Solved Kepler's equation using Newton–Raphson iteration.</li>
          <li>Computed Classical Orbital Elements (COEs).</li>
          <li>Verified conservation of orbital energy & angular momentum.</li>
          <li>Transformed states between perifocal & ECI reference frames.</li>
        </ul>
      </div>

      <a href="kepler-solver.html" class="project-button">
        View More Details
      </a>
    </div>
  </div>

  <div class="project-card">
    <div class="project-media">
      <img src="images/cessna.png" alt="Closed-Loop Pitch Controller">
      <p style="font-size: 0.78em; color: #64748b !important; margin-top: 5px; font-style: italic; margin-bottom: 0;">
        Closed-Loop Pitch Controller in Action
      </p>
    </div>

    <div class="project-text">
      <div>
        <h3>Pitch Autopilot Controller Model</h3>
        <ul>
          <li>Designed PID controller with anti-windup & actuator dynamics.</li>
          <li>Implemented Kalman filtering for robust state estimation.</li>
          <li>Evaluated performance using step, doublet, & square-wave inputs.</li>
          <li>Visualized response through real-time FlightGear 6DOF simulation.</li>
        </ul>
      </div>

      <a href="pitch-controller.html" class="project-button">
        View More Details
      </a>
    </div>
  </div>

</div>
