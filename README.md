<style>
  /* GLOBAL FONT OVERRIDES */
  body, p, li, a, span, button, td, div {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif !important;
    color: #334155;
    line-height: 1.55;
  }

  .about-text, .about-text p {
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif !important;
    color: #334155 !important;
    font-size: 0.95em !important;
    line-height: 1.6 !important;
  }

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

  /* --- GRID LAYOUT --- */
  .projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 460px));
    gap: 24px;
    margin-top: 14px;
    margin-bottom: 28px;
  }

  /* --- TRUE GLASSMORPHISM CARDS --- */
  .project-card {
    /* Frost tint & high blur */
    background: rgba(255, 255, 255, 0.45) !important;
    backdrop-filter: blur(16px) saturate(180%) !important;
    -webkit-backdrop-filter: blur(16px) saturate(180%) !important;
    
    /* Crisp glass borders & drop shadow */
    border: 1px solid rgba(255, 255, 255, 0.8) !important;
    border-bottom: 1px solid rgba(222, 226, 230, 0.6) !important;
    border-radius: 16px;
    padding: 20px;
    
    /* Multi-layered glass shadow for depth */
    box-shadow: 0 10px 30px -5px rgba(0, 0, 0, 0.08), 
                inset 0 1px 0 0 rgba(255, 255, 255, 0.9) !important;
    
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
  }

  .project-card:hover {
    transform: translateY(-4px);
    background: rgba(255, 255, 255, 0.6) !important;
    box-shadow: 0 20px 40px -10px rgba(0, 0, 0, 0.12), 
                inset 0 1px 0 0 rgba(255, 255, 255, 1) !important;
    border-color: rgba(37, 99, 235, 0.3) !important;
  }

  /* IMAGE CONTAINMENT */
  .project-media {
    text-align: center;
    border: none !important;
    margin-bottom: 12px;
    background: rgba(255, 255, 255, 0.3);
    border-radius: 10px;
    padding: 8px;
  }

  .project-media img {
    width: 100%;
    height: auto;
    max-height: 200px;
    object-fit: contain;
    border-radius: 6px;
    display: block;
    margin: 0 auto;
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

  h2, h3, p { margin-top: 0; }
  img, div, section { border: none !important; }

  .main-content {
    max-width: 1400px !important;
    width: 92% !important;
    margin: 0 auto !important;
  }

  /* BUTTON STYLING */
  .project-button {
    display: inline-block;
    align-self: flex-start;
    margin-top: 12px;
    padding: 8px 16px;
    border: 1px solid rgba(37, 99, 235, 0.4);
    border-radius: 8px;
    color: #2563eb !important;
    text-decoration: none !important;
    font-weight: 600 !important;
    font-size: 0.85em;
    background: rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(4px);
    transition: all 0.2s ease;
  }

  .project-button:hover {
    background-color: #2563eb;
    color: #ffffff !important;
    box-shadow: 0 4px 12px rgba(37, 99, 235, 0.25);
  }

  /* BULLETS */
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

  /* SKILLS */
  .skill-group { margin-bottom: 18px; }
  .skill-group h3 {
    margin-bottom: 8px;
    color: #475569 !important;
    font-size: 1.05em;
    font-weight: 600 !important;
  }

  .skill-pills {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  /* --- GLASS SKILL PILLS --- */
  .skill-pill {
    display: inline-block;
    padding: 6px 14px;
    background: rgba(255, 255, 255, 0.6);
    backdrop-filter: blur(10px);
    -webkit-backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.8);
    box-shadow: 0 2px 5px rgba(0,0,0,0.03), inset 0 1px 0 rgba(255,255,255,0.8);
    border-radius: 20px;
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
    0%, 60% {
      background-color: rgba(255, 255, 255, 0.95);
      border-color: var(--glow-color);
      box-shadow: 0 0 12px var(--glow-color);
      transform: translateY(-2px);
      color: var(--glow-color) !important;
      font-weight: 600 !important;
    }
    100% {
      background: rgba(255, 255, 255, 0.6);
      border-color: rgba(255, 255, 255, 0.8);
      box-shadow: 0 2px 5px rgba(0,0,0,0.03);
      transform: translateY(0);
      color: #334155 !important;
      font-weight: 500 !important;
    }
  }

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
