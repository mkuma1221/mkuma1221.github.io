<style>
  .page-header {
    background-image: url('GAX.jpg') !important;
    background-size: cover !important;
    background-position: center !important;
  }
  
  /* Flexbox Container to replace tables and remove all borders */
  .project-container {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    align-items: flex-start;
    border: none !important;
    margin-top: 20px;
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
</style>

<h2 style="color: #000080; font-size: 1.8em; margin-top: 30px; margin-bottom: 15px; font-family: sans-serif;">About Me</h2>

<p style="color: #444; line-height: 1.6; font-family: sans-serif; margin-bottom: 30px;">
  Hi, my name is Mohana Kumanan, and I am an aerospace engineering student with a focus on control systems and orbital mechanics. I have experience in both technical analysis and collaborative engineering projects, with a strong interest in applying aerospace engineering principles to real-world systems. Through my coursework and projects, I have developed a solid foundation in orbital mechanics, dynamics, and control systems, along with practical experience in MATLAB, numerical methods, system modeling, and spacecraft state propagation. These experiences have strengthened my ability to analyze complex engineering problems, develop computational solutions, and validate results through analytical and numerical techniques. This website serves as both a technical portfolio and a professional archive, documenting the methodologies, analysis, and engineering concepts developed throughout my projects while showcasing the technical experience and skills I have gained.
</p>

<h2 style="color: #000080; font-size: 1.8em; margin-bottom: 20px; font-family: sans-serif;">Projects</h2>

<h3 style="color: #000080; font-size: 1.4em; margin-top: 30px; margin-bottom: 25px; text-align: center; font-family: sans-serif; border: none !important;">
  Kepler’s Problem Solver & Orbital Verification
</h3>

<div class="project-container">
  <div class="project-text">
    <p style="color: #444; line-height: 1.6; margin-top: 0; margin-bottom: 8px; font-family: sans-serif;">
      Developed a MATLAB orbital mechanics simulation to solve Kepler’s equation using the Newton–Raphson iterative method. The project computed Classical Orbital Elements from given position, velocity, and gravitational parameter, verified results through conservation of orbital energy and angular momentum, and used Direction Cosine Matrices to transform states between perifocal and ECI reference frames.
    </p>
    <a href="INSERT_YOUR_GITHUB_OR_PAGE_LINK_HERE" style="font-family: sans-serif; text-decoration: none; color: #007bff; font-weight: bold; display: inline-block; margin-top: 5px;">View More Details</a>
  </div>
  
  <div class="project-media">
    <img src="SAT.png" alt="Satellite Trajectory" style="width: 100%; max-width: 450px; height: auto; display: block; margin: 0 auto; border: none !important; border-radius: 4px;">
    <p style="font-size: 0.85em; color: #666; margin-top: 8px; font-family: sans-serif; font-style: italic;">
      Comparison of Newton Raphson to ODE 45
    </p>
  </div>
</div>
