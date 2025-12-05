<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Dhruv Manohar Patel | Full Stack .NET Developer</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Dhruv Manohar Patel - Full Stack .NET Developer, Backend Specialist, MCA Graduate">
  <link rel="icon" href="https://avatars.githubusercontent.com/u/0?v=4">

  <!-- Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

  <style>
    :root {
      --primary: #0d6efd;
      --primary-dark: #084298;
      --light: #f4f8ff;
      --dark: #0a2540;
      --text: #1f2933;
      --card-bg: #ffffff;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      scroll-behavior: smooth;
    }

    body {
      font-family: "Segoe UI", system-ui, sans-serif;
      background: linear-gradient(180deg, #f4f8ff, #ffffff);
      color: var(--text);
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: var(--primary);
      font-weight: 600;
    }

    section {
      max-width: 1100px;
      margin: auto;
      padding: 90px 20px;
    }

    h1, h2, h3 {
      color: var(--dark);
      margin-bottom: 10px;
    }

    h2 {
      font-size: 2.2rem;
      margin-bottom: 35px;
      font-weight: 800;
    }

    /* HERO */
    .hero {
      text-align: center;
      padding: 120px 20px 80px;
      background: linear-gradient(135deg, var(--primary), var(--primary-dark));
      color: white;
    }

    .hero img {
      border-radius: 50%;
      border: 4px solid white;
      width: 150px;
      margin-bottom: 15px;
    }

    .hero h1 {
      font-size: 2.8rem;
      color: white;
    }

    .hero h3 {
      font-weight: 500;
      opacity: 0.9;
    }

    .socials {
      margin-top: 20px;
    }

    .socials a {
      margin: 0 10px;
      color: white;
      font-size: 22px;
    }

    /* NAVBAR */
    .navbar {
      text-align: center;
      padding: 15px;
      position: sticky;
      top: 0;
      background: white;
      border-bottom: 1px solid #e5e7eb;
      z-index: 100;
    }

    .navbar a {
      margin: 0 10px;
      font-size: 15px;
      color: var(--primary);
    }

    .navbar i {
      margin-right: 5px;
    }

    /* UNIFIED CARD */
    .section-card {
      background: var(--card-bg);
      padding: 25px;
      margin-bottom: 25px;
      border-radius: 14px;
      box-shadow: 0 10px 25px rgba(13,110,253,0.12);
      border-left: 5px solid var(--primary);
      transition: transform 0.25s ease;
    }

    .section-card:hover {
      transform: translateY(-4px);
    }

    .section-card h3 i {
      color: var(--primary);
      margin-right: 6px;
    }

    /* SKILLS */
    .skills img {
      width: 65%;
      max-width: 420px;
    }

    /* LISTS */
    ul {
      padding-left: 20px;
      margin-top: 10px;
    }

    li {
      margin-bottom: 6px;
    }

    /* FOOTER */
    footer {
      text-align: center;
      padding: 50px 20px;
      font-size: 14px;
      color: #475569;
      background: #f1f5ff;
      border-top: 1px solid #dbeafe;
    }

    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2.1rem;
      }
      .skills img {
        width: 95%;
      }
    }
  </style>
</head>

<body>

  <!-- HERO -->
  <div class="hero" id="home">
    <img src="https://avatars.githubusercontent.com/u/0?v=4">
    <h1><i class="fa-solid fa-user"></i> Dhruv Manohar Patel</h1>
    <h3>Full Stack .NET Developer • Backend Specialist • MCA Graduate</h3>

    <div class="socials">
      <a href="https://linkedin.com/in/dhruvpateltural"><i class="fab fa-linkedin"></i></a>
      <a href="https://github.com/dhruvpateltural"><i class="fab fa-github"></i></a>
      <a href="mailto:dhruvpateltural@gmail.com"><i class="fa-solid fa-envelope"></i></a>
    </div>
  </div>

  <!-- NAVBAR -->
  <div class="navbar">
    <a href="#about"><i class="fa-user"></i>About</a>
    <a href="#skills"><i class="fa-code"></i>Skills</a>
    <a href="#internship"><i class="fa-briefcase"></i>Internship</a>
    <a href="#projects"><i class="fa-diagram-project"></i>Projects</a>
    <a href="#education"><i class="fa-graduation-cap"></i>Education</a>
    <a href="#certifications"><i class="fa-certificate"></i>Certifications</a>
    <a href="#achievements"><i class="fa-trophy"></i>Achievements</a>
  </div>

  <!-- ABOUT -->
  <section id="about">
    <h2><i class="fa-user"></i> About Me</h2>
    <div class="section-card">
      MCA graduate with <b>full-stack development</b> experience using  
      <b>C#, ASP.NET, SQL Server & Entity Framework</b>.  
      I build <b>secure, scalable backend systems</b>, optimize databases,  
      and work efficiently in <b>Agile SDLC environments</b>.
    </div>
  </section>

  <!-- SKILLS -->
  <section id="skills" class="skills">
    <h2><i class="fa-code"></i> Tech Stack</h2>
    <div class="section-card" style="text-align:center;">
      <img src="https://skillicons.dev/icons?i=cs,dotnet,java,html,css,js,git,github,visualstudio,mysql">
    </div>
  </section>

  <!-- INTERNSHIP -->
  <section id="internship">
    <h2><i class="fa-briefcase"></i> Internship</h2>
    <div class="section-card">
      <h3><i class="fa-building"></i> Software Development Intern — Aaryak Solutions</h3>
      <p><b>Jan 2025 – Jun 2025</b></p>
      <ul>
        <li>Developed 10+ backend modules</li>
        <li>Improved SQL performance by 20–30%</li>
        <li>Implemented RBAC-based security</li>
        <li>Worked in Agile SDLC lifecycle</li>
      </ul>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="projects">
    <h2><i class="fa-diagram-project"></i> Projects</h2>

    <div class="section-card">
      <h3><i class="fa-utensils"></i> Restaurant Management System</h3>
      <p><b>Tech:</b> C#, ASP.NET, SQL Server, EF, HTML, CSS</p>
      <ul>
        <li>Billing, Orders & Inventory Automation</li>
        <li>Secure Role-Based Authentication</li>
        <li>Optimized Backend APIs</li>
      </ul>
    </div>

    <div class="section-card">
      <h3><i class="fa-gears"></i> Hardware Shop Management System</h3>
      <p><b>Tech:</b> WinForms, C#, SQL Server, EF</p>
      <ul>
        <li>Sales & Inventory Automation</li>
        <li>ORM-based Reliable Data Handling</li>
      </ul>
    </div>
  </section>

  <!-- EDUCATION -->
  <section id="education">
    <h2><i class="fa-graduation-cap"></i> Education</h2>

    <div class="section-card">
      <h3>MCA — Finolex Academy</h3>
      <p>2025</p>
      <b>CGPA: 8.4</b>
    </div>

    <div class="section-card">
      <h3>B.Com — Gogate Jogalekar College</h3>
      <p>2023</p>
      <b>CGPA: 8.78</b>
    </div>
  </section>

  <!-- CERTIFICATIONS -->
  <section id="certifications">
    <h2><i class="fa-certificate"></i> Certifications</h2>
    <div class="section-card">
      <ul>
        <li>Java Programming Fundamentals — SpringBoard</li>
        <li>Cyber Security & Privacy Fundamentals — NPTEL</li>
        <li>Web Development Fundamentals — IBM</li>
      </ul>
    </div>
  </section>

  <!-- ACHIEVEMENTS -->
  <section id="achievements">
    <h2><i class="fa-trophy"></i> Achievements</h2>

    <div class="section-card">
      <ul>
        <li>Marketing Lead — Excellentia 2K25</li>
        <li>Photography & Videography Coordinator — Finolex MCA Dept</li>
      </ul>
    </div>

    <h3 style="margin-top:20px;">Core Strengths</h3>
    <div class="section-card">
      <ul>
        <li>Problem Solving</li>
        <li>Agile Collaboration</li>
        <li>Analytical Thinking</li>
        <li>Time Management</li>
      </ul>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    ⭐ If you like my work, consider starring my repositories and connecting with me.
    <br><br>
    © 2025 Dhruv Manohar Patel
  </footer>

</body>
</html>
