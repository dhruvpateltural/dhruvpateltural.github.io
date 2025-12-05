
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Dhruv Manohar Patel | Full Stack .NET Developer</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="Dhruv Manohar Patel - Full Stack .NET Developer, Backend Specialist, MCA Graduate"/>
  <link rel="icon" href="https://avatars.githubusercontent.com/u/0?v=4"/>

  <style>
    :root {
      --primary: #0d6efd;
      --dark: #111;
      --light: #f9f9f9;
      --text: #333;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      scroll-behavior: smooth;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
      background: var(--light);
      color: var(--text);
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: var(--primary);
      font-weight: 500;
    }

    section {
      max-width: 1000px;
      margin: auto;
      padding: 70px 20px;
    }

    h1, h2, h3 {
      color: var(--dark);
      margin-bottom: 10px;
    }

    h2 {
      font-size: 2rem;
      margin-bottom: 25px;
    }

    /* HERO */
    .hero {
      text-align: center;
      padding: 100px 20px 70px;
      background: white;
    }

    .hero img {
      border-radius: 50%;
      border: 4px solid var(--primary);
      width: 140px;
      margin-bottom: 15px;
    }

    .hero h1 {
      font-size: 2.4rem;
    }

    .hero h3 {
      font-weight: 500;
      color: #555;
    }

    /* NAVBAR */
    .navbar {
      text-align: center;
      padding: 15px;
      position: sticky;
      top: 0;
      background: white;
      border-bottom: 1px solid #eee;
      z-index: 100;
    }

    .navbar a {
      margin: 0 8px;
      font-size: 15px;
    }

    /* SOCIALS */
    .socials {
      margin-top: 20px;
      text-align: center;
    }

    .socials img {
      margin: 6px;
      height: 28px;
    }

    /* SKILLS */
    .skills img {
      width: 60%;
      max-width: 400px;
      margin-top: 10px;
    }

    /* UNIFIED CARD STYLE (EDUCATION STYLE EVERYWHERE) */
    .section-card {
      background: white;
      padding: 20px;
      margin-bottom: 20px;
      border-radius: 14px;
      box-shadow: 0 6px 16px rgba(0,0,0,0.05);
      border-left: 4px solid var(--primary);
    }

    /* FOOTER */
    footer {
      text-align: center;
      padding: 40px 20px;
      font-size: 14px;
      color: #666;
    }

    @media (max-width: 768px) {
      .hero h1 {
        font-size: 2rem;
      }
      .skills img {
        width: 90%;
      }
    }
  </style>
</head>

<body>

  <!-- HERO -->
  <div class="hero" id="home">
    <img src="https://avatars.githubusercontent.com/u/0?v=4" alt="Dhruv Patel">
    <h1>Dhruv Manohar Patel</h1>
    <h3>Full Stack .NET Developer • Backend Specialist • MCA Graduate</h3>

    <div class="socials">
      <a href="https://linkedin.com/in/dhruvpateltural" target="_blank">
        <img src="https://img.shields.io/badge/LinkedIn-0d6efd?style=flat&logo=linkedin&logoColor=white">
      </a>
      <a href="https://github.com/dhruvpateltural" target="_blank">
        <img src="https://img.shields.io/badge/GitHub-111111?style=flat&logo=github&logoColor=white">
      </a>
      <a href="mailto:dhruvpateltural@gmail.com">
        <img src="https://img.shields.io/badge/Email-0d6efd?style=flat&logo=gmail&logoColor=white">
      </a>
    </div>
  </div>

  <!-- NAVBAR -->
  <div class="navbar">
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#internship">Internship</a>
    <a href="#projects">Projects</a>
    <a href="#education">Education</a>
    <a href="#certifications">Certifications</a>
    <a href="#achievements">Achievements</a>
  </div>

  <!-- ABOUT -->
  <section id="about">
    <h2>About Me</h2>
    <div class="section-card">
      <p>
        MCA graduate with hands-on experience in <strong>full-stack development</strong>,
        specializing in <strong>C#, ASP.NET, SQL Server, and Entity Framework</strong>.
        I build <strong>secure, scalable backend systems</strong>, optimize databases,
        and work efficiently in <strong>Agile SDLC environments</strong>.
      </p>
    </div>
  </section>

  <!-- SKILLS -->
  <section id="skills" class="skills">
    <h2>Tech Stack</h2>
    <div class="section-card" style="text-align:center;">
      <img src="https://skillicons.dev/icons?i=cs,dotnet,java,html,css,js,git,github,visualstudio,mysql">
    </div>
  </section>

  <!-- INTERNSHIP -->
  <section id="internship">
    <h2>Internship</h2>

    <div class="section-card">
      <h3>Software Development Intern — Aaryak Solutions</h3>
      <p><strong>Jan 2025 – Jun 2025</strong></p>
      <ul>
        <li>Developed 10+ backend modules</li>
        <li>Improved SQL performance by 20–30%</li>
        <li>Implemented RBAC-based authentication</li>
        <li>Worked across full Agile SDLC lifecycle</li>
      </ul>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="projects">
    <h2>Projects</h2>

    <div class="section-card">
      <h3>Restaurant Management System</h3>
      <p><strong>Tech:</strong> C#, ASP.NET, SQL Server, Entity Framework, HTML, CSS</p>
      <ul>
        <li>Billing, Orders & Inventory Automation</li>
        <li>Secure Role-Based Authentication</li>
        <li>Optimized Backend APIs</li>
      </ul>
    </div>

    <div class="section-card">
      <h3>Hardware Shop Management System</h3>
      <p><strong>Tech:</strong> WinForms, C#, SQL Server, Entity Framework</p>
      <ul>
        <li>Sales & Inventory Automation</li>
        <li>ORM-based Reliable Data Handling</li>
      </ul>
    </div>
  </section>

  <!-- EDUCATION -->
  <section id="education">
    <h2>Education</h2>

    <div class="section-card">
      <h3>Master of Computer Applications (MCA)</h3>
      <p>Finolex Academy — 2025</p>
      <p><strong>CGPA:</strong> 8.4</p>
    </div>

    <div class="section-card">
      <h3>Bachelor of Commerce (B.Com)</h3>
      <p>Gogate Jogalekar College — 2023</p>
      <p><strong>CGPA:</strong> 8.78</p>
    </div>
  </section>

  <!-- CERTIFICATIONS -->
  <section id="certifications">
    <h2>Certifications</h2>
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
    <h2>Achievements</h2>

    <div class="section-card">
      <ul>
        <li><strong>Marketing Lead — Excellentia 2K25</strong></li>
        <li><strong>Photography & Videography Coordinator — Finolex MCA Dept</strong></li>
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
