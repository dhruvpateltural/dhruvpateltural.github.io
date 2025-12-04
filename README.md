
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Dhruv Manohar Patel | Full Stack .NET Developer</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

  <style>
    * { margin: 0; padding: 0; box-sizing: border-box }

    :root {
      --primary: #0d6efd;
      --secondary: #6f42c1;
      --accent: #00e5ff;
      --bg-dark: #060b23;
      --glass: rgba(255,255,255,0.06);
      --border: rgba(255,255,255,0.15);
      --text: #e8e9f3;
    }

    body {
      font-family: 'Inter', sans-serif;
      background: radial-gradient(1200px 600px at 10% 10%, #11186b, transparent),
                  radial-gradient(1000px 500px at 90% 90%, #2a0d52, transparent),
                  var(--bg-dark);
      color: var(--text);
    }

    section {
      max-width: 1200px;
      margin: auto;
      padding: 6rem 2rem;
    }

    h1 {
      font-size: 3.8rem;
      background: linear-gradient(90deg, var(--primary), var(--secondary));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 1rem;
    }

    h2 {
      font-size: 2.4rem;
      text-align: center;
      margin-bottom: 3rem;
      background: linear-gradient(90deg, var(--primary), var(--secondary));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    /* NAV */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      padding: 1rem 5%;
      backdrop-filter: blur(16px);
      background: rgba(5,8,17,0.7);
      z-index: 1000;
    }

    nav ul {
      display: flex;
      justify-content: center;
      gap: 2rem;
      list-style: none;
    }

    nav a {
      color: var(--text);
      text-decoration: none;
      font-weight: 500;
      position: relative;
    }

    nav a::after {
      content: '';
      position: absolute;
      bottom: -6px;
      left: 0;
      width: 0;
      height: 2px;
      background: linear-gradient(90deg, var(--primary), var(--secondary));
      transition: 0.3s;
    }

    nav a:hover::after { width: 100%; }

    /* HERO */
    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
    }

    .hero-content {
      background: var(--glass);
      border: 1px solid var(--border);
      padding: 4rem;
      border-radius: 24px;
      box-shadow: 0 40px 100px rgba(0,0,0,0.6);
      animation: zoom 1s ease;
    }

    @keyframes zoom {
      from { opacity: 0; transform: scale(0.95); }
      to { opacity: 1; transform: scale(1); }
    }

    .subtitle {
      color: var(--accent);
      font-size: 1.5rem;
      margin-bottom: 2rem;
    }

    .social-links a {
      padding: 14px 32px;
      border-radius: 40px;
      background: linear-gradient(135deg, var(--primary), var(--secondary));
      text-decoration: none;
      color: #fff;
      margin: 0.5rem;
      display: inline-block;
      transition: 0.3s;
      font-weight: 600;
      box-shadow: 0 10px 30px rgba(13,110,253,0.4);
    }

    .social-links a:hover {
      transform: translateY(-5px);
      box-shadow: 0 20px 60px rgba(13,110,253,0.7);
    }

    /* CARDS */
    .card {
      background: var(--glass);
      border: 1px solid var(--border);
      border-radius: 24px;
      padding: 2.5rem;
      margin-bottom: 2rem;
      box-shadow: 0 20px 60px rgba(0,0,0,0.4);
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-8px);
      box-shadow: 0 30px 90px rgba(111,66,193,0.5);
    }

    /* SKILLS */
    .skills {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(140px,1fr));
      gap: 2rem;
      text-align: center;
    }

    .skill {
      background: var(--glass);
      padding: 1.8rem;
      border-radius: 18px;
      border: 1px solid var(--border);
      transition: 0.3s;
    }

    .skill:hover {
      transform: scale(1.1);
      background: linear-gradient(135deg, rgba(13,110,253,0.25), rgba(111,66,193,0.25));
    }

    /* PROJECTS */
    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(320px,1fr));
      gap: 2rem;
    }

    .project {
      background: linear-gradient(135deg, rgba(13,110,253,0.15), rgba(111,66,193,0.15));
      border-radius: 22px;
      padding: 2.5rem;
      border: 1px solid var(--border);
      transition: 0.3s;
    }

    .project:hover {
      transform: translateY(-10px);
      box-shadow: 0 30px 90px rgba(111,66,193,0.6);
    }

    /* TABLE */
    table {
      width: 100%;
      border-collapse: collapse;
    }

    th, td {
      padding: 1rem;
      border-bottom: 1px solid var(--border);
    }

    th {
      color: var(--accent);
    }

    /* FOOTER */
    footer {
      text-align: center;
      padding: 4rem 2rem;
      background: rgba(0,0,0,0.3);
    }

    @media (max-width: 768px) {
      h1 { font-size: 2.5rem }
      .subtitle { font-size: 1.1rem }
    }
  </style>
</head>

<body>

<!-- NAV -->
<nav>
  <ul>
    <li><a href="#about">About</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#internship">Experience</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#education">Education</a></li>
    <li><a href="#achievements">Achievements</a></li>
  </ul>
</nav>

<!-- HERO -->
<div class="hero">
  <div class="hero-content">
    <h1>Dhruv Manohar Patel</h1>
    <p class="subtitle">Full Stack .NET Developer | Backend Specialist | MCA Graduate</p>
    <div class="social-links">
      <a href="https://linkedin.com/in/dhruvpateltural">LinkedIn</a>
      <a href="https://github.com/dhruvpateltural">GitHub</a>
      <a href="mailto:dhruvpateltural@gmail.com">Email</a>
    </div>
  </div>
</div>

<section id="about">
  <h2>About Me</h2>
  <div class="card">
    MCA graduate specializing in **C#, ASP.NET, SQL Server, and Entity Framework** with strong focus on **secure, scalable enterprise software** and **database optimization**.
  </div>
</section>

<section id="skills">
  <h2>Tech Stack</h2>
  <div class="skills">
    <div class="skill">C#</div>
    <div class="skill">.NET</div>
    <div class="skill">Java</div>
    <div class="skill">SQL Server</div>
    <div class="skill">Entity Framework</div>
    <div class="skill">HTML/CSS</div>
    <div class="skill">JavaScript</div>
    <div class="skill">Git</div>
  </div>
</section>

<section id="projects">
  <h2>Projects</h2>
  <div class="projects">
    <div class="project">
      <h3>Restaurant Management System</h3>
      Billing, Orders, Inventory, RBAC Authentication, Performance APIs
    </div>
    <div class="project">
      <h3>Hardware Shop Management</h3>
      Sales & Inventory Automation using WinForms & SQL Server
    </div>
  </div>
</section>

<section id="education">
  <h2>Education</h2>
  <div class="card">
    <table>
      <tr><th>Degree</th><th>Institution</th><th>Year</th><th>CGPA</th></tr>
      <tr><td>MCA</td><td>Finolex Academy</td><td>2025</td><td>8.4</td></tr>
      <tr><td>B.Com</td><td>Gogate Jogalekar College</td><td>2023</td><td>8.78</td></tr>
    </table>
  </div>
</section>

<footer>
  <h3>Career Objective</h3>
  To work as a <strong>Full Stack .NET Developer</strong> building <strong>secure, scalable enterprise applications</strong>.
</footer>

</body>
</html>
