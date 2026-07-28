<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet">

<style>

/* ---------------- GLOBAL TYPOGRAPHY ---------------- */

body,
p,
li,
a,
span,
button,
td,
div{
    font-family:'Inter',-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,sans-serif!important;
    color:#334155;
    line-height:1.6;
}

.about-text,
.about-text p{
    font-family:'Inter',-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,sans-serif!important;
    color:#334155!important;
    font-size:.95em!important;
    line-height:1.65!important;
}

h1,
h2,
h3,
h4{
    font-family:'Plus Jakarta Sans',sans-serif!important;
    color:#1e293b!important;
    font-weight:700!important;
}

.page-header{
    background-image:url('images/GAX.jpg')!important;
    background-size:cover!important;
    background-position:center!important;
}


/* ---------------- PAGE WIDTH ---------------- */

.main-content{
    max-width:1400px!important;
    width:92%!important;
    margin:0 auto!important;
}

img,
div,
section{
    border:none!important;
}

h2,
h3,
p{
    margin-top:0;
}


/* ---------------- PROJECT GRID ---------------- */

.projects-grid{

    display:grid;

    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));

    gap:16px;

    margin-top:16px;

    margin-bottom:26px;

}


/* ---------------- PROJECT CARD ---------------- */

.project-card{

    background:#ffffff;

    border:1px solid #dbe4ee!important;

    border-radius:12px;

    padding:16px;

    box-shadow:
        0 10px 28px rgba(15,23,42,.06),
        0 2px 8px rgba(15,23,42,.04);

    display:flex;

    flex-direction:column;

    justify-content:space-between;

}


/* ---------------- PROJECT IMAGE ---------------- */

.project-media{

    text-align:center;

    margin-bottom:14px;

}

.project-media img{

    width:100%;

    max-width:360px;

    height:auto;

    display:block;

    margin:0 auto;

    border-radius:8px;

    box-shadow:0 2px 6px rgba(0,0,0,.08);

}


/* ---------------- PROJECT TEXT ---------------- */

.project-text{

    display:flex;

    flex-direction:column;

    justify-content:space-between;

    flex-grow:1;

}

.project-card h3{

    font-size:1.15em!important;

    line-height:1.35;

    margin-bottom:10px;

}

.project-text ul{

    list-style-type:square;

    padding-left:18px;

    margin-top:4px;

    margin-bottom:14px;

}

.project-text li{

    margin-bottom:6px;

    font-size:.88em;

    color:#475569!important;

}


/* ---------------- BUTTON ---------------- */

.project-button{

    display:inline-block;

    align-self:flex-start;

    margin-top:8px;

    padding:8px 16px;

    border:2px solid #2563eb;

    border-radius:8px;

    color:#2563eb!important;

    text-decoration:none!important;

    font-size:.85em;

    font-weight:600!important;

    transition:.2s;

}

.project-button:hover{

    background:#2563eb;

    color:white!important;

}


/* ---------------- SKILLS ---------------- */

.skill-group{

    margin-bottom:18px;

}

.skill-group h3{

    color:#475569!important;

    margin-bottom:8px;

    font-size:1.05em;

}

.skill-pills{

    display:flex;

    flex-wrap:wrap;

    gap:8px;

}

.skill-pill{

    display:inline-block;

    padding:5px 12px;

    border-radius:14px;

    background:#f8fafc;

    border:1px solid #cbd5e1;

    color:#334155!important;

    font-size:.85em;

    font-weight:500!important;

    transition:.3s;

    cursor:pointer;

}

.skill-pill:hover{

    animation:temporaryGlow 1.5s ease-out forwards;

}

@keyframes temporaryGlow{

0%{

background:white;

border-color:var(--glow-color);

box-shadow:0 0 10px var(--glow-color);

transform:translateY(-2px);

color:var(--glow-color)!important;

font-weight:600!important;

}

60%{

background:white;

border-color:var(--glow-color);

box-shadow:0 0 10px var(--glow-color);

transform:translateY(-2px);

color:var(--glow-color)!important;

font-weight:600!important;

}

100%{

background:#f8fafc;

border-color:#cbd5e1;

box-shadow:none;

transform:none;

color:#334155!important;

font-weight:500!important;

}

}

.skill-pill.matlab{--glow-color:#e05206;}
.skill-pill.python{--glow-color:#306998;}
.skill-pill.cpp{--glow-color:#00599c;}
.skill-pill.simulink{--glow-color:#0076a8;}
.skill-pill.stateflow{--glow-color:#008080;}
.skill-pill.solidworks{--glow-color:#d12727;}
.skill-pill.ansys{--glow-color:#e6a100;}
.skill-pill.flightgear{--glow-color:#009999;}
.skill-pill.starccm{--glow-color:#00a3a6;}
.skill-pill.altium{--glow-color:#cc9900;}

</style>

<table style="width:100%;border-collapse:collapse;border:none;margin-bottom:30px;">

<tr>

<td style="width:60%;padding-right:35px;border:none;vertical-align:top;" class="about-text">

<h2 style="font-size:1.8em;margin-top:20px;margin-bottom:12px;">
About Me
</h2>

<p>

Hi, my name is Mohana Kumanan, and I am an aerospace engineering student with an interest in control systems and orbital mechanics. I have experience in technical analysis, collaborative engineering projects, MATLAB, Simulink, numerical methods, and spacecraft dynamics. This website serves as a technical portfolio documenting the engineering methodologies, analyses, and computational tools developed throughout my projects.

</p>

</td>

<td style="width:40%;border:none;vertical-align:top;">

<h2 style="font-size:1.8em;margin-top:20px;margin-bottom:18px;">
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

<h2 style="font-size:1.8em;margin-bottom:12px;">
Projects
</h2>

<div class="projects-grid">
  <!-- ==================== PROJECT 1 ==================== -->

  <div class="project-card">

    <div class="project-media">

      <img src="images/SAT.png" alt="Satellite Trajectory">

      <p style="font-size:0.8em;color:#64748b!important;margin-top:6px;font-style:italic;">
        Comparison of Newton-Raphson to ODE45
      </p>

    </div>

    <div class="project-text">

      <div>

        <h3>Kepler’s Problem Solver &amp; Orbital Propagation</h3>

        <ul>
          <li>Solved Kepler's equation using the Newton–Raphson iterative method.</li>
          <li>Computed Classical Orbital Elements (COEs).</li>
          <li>Verified conservation of orbital energy and angular momentum.</li>
          <li>Transformed states between perifocal and ECI reference frames.</li>
        </ul>

      </div>

      <a href="kepler-solver.html" class="project-button">
        View More Details
      </a>

    </div>

  </div>


  <!-- ==================== PROJECT 2 ==================== -->

  <div class="project-card">

    <div class="project-media">

      <img src="images/cessna.png" alt="Closed-Loop Pitch Controller">

      <p style="font-size:0.8em;color:#64748b!important;margin-top:6px;font-style:italic;">
        Closed-Loop Pitch Controller in Action
      </p>

    </div>

    <div class="project-text">

      <div>

        <h3>Pitch Autopilot Controller Model</h3>

        <ul>
          <li>Designed a PID controller with anti-windup and actuator dynamics.</li>
          <li>Implemented Kalman filtering for robust state estimation.</li>
          <li>Evaluated controller performance using step, doublet, and square-wave inputs.</li>
          <li>Visualized aircraft response through real-time FlightGear 6DOF simulation.</li>
        </ul>

      </div>

      <a href="pitch-controller.html" class="project-button">
        View More Details
      </a>

    </div>

  </div>

</div>
