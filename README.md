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

  /* --- SLIGHTLY LARGER GRID LAYOUT FOR PROJECTS --- */
  .projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 460px)); /* Expanded width for slightly bigger cards */
    gap: 20px;
    margin-top: 14px;
    margin-bottom: 28px;
  }

  /* SHADED CARDS (STATIONARY - NO HOVER MOVEMENT) */
  .project-card {
    background-color: #f8fafc; /* Subtle shading */
    border: 1px solid #e2e8f0 !important;
    border-radius: 12px;
    padding: 16px; /* Comfortably sized padding */
    box-shadow: 0 1px 4px rgba(0, 0, 0, 0.05);
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  /* FIXED IMAGE CONTAINER */
  .project-media {
    text-align: center;
    border: none !important;
    margin-bottom: 10px;
    width: 100%;
    height: 200px; /* Fixed height container for consistent card sizing */
    overflow: hidden;
    border-radius: 8px;
    box-shadow: 0 1px 4px rgba(0, 0, 0, 0.08);
    background-color: #ffffff; /* Clean white background behind contained images */
  }

  .project-media img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }

  /* SPECIFIC FIT FOR LEFT GRAPH (Prevents cropping axis & legend) */
  .project-media img.sat-img {
    object-fit: contain !important;
    padding: 6px; /* Padding ensures plot labels/legend are fully visible */
    box-sizing: border-box;
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

  /* Hover glow animation for skill pills */
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
</style>

<table style="width:100%; border-collapse:collapse; border:none; margin-bottom:30px;">
  <tr>
    <td style="width:60%; vertical-align:top; padding-right:35px; border:none;" class="about-text">
      <h2 style="font-size:1.8em; margin-top:20px; margin-bottom:12px;">
        About Me
      </h2>
      <p style="margin-bottom:0;">
       Hi, I'm Mohana Kumanan, an aerospace engineering student with a primary focus on Guidance, Navigation, and Control (GNC), orbital mechanics, and aerospace structures. My experience centers on technical analysis, spacecraft dynamics, and computational modeling. I regularly use MATLAB, Simulink, and numerical methods to model, analyze, and validate complex aerospace systems. This portfolio showcases the computational tools, engineering methodologies, and technical projects I have developed throughout my academic and personal work. This portfolio will continue to grow as I complete new projects. If you have any feedback or would like to connect, please feel free to reach out.
      </p>
    </td>

    <td style="width:40%; vertical-align:top; border:none;">
      <h2 style="font-size:1.8em; margin-top:20px; margin-bottom:18px;">
        Technical Skills
