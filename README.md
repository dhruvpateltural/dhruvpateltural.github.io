
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Dhruv Manohar Patel | Full Stack .NET Developer</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

 <style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    :root {
        --primary: #0d6efd;
        --secondary: #6f42c1;
        --dark: #0a0e27;
        --darker: #050811;
        --light: #e8e9f3;
        --accent: #00d4ff;
    }

    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background: linear-gradient(135deg, var(--darker) 0%, var(--dark) 100%);
        color: var(--light);
        overflow-x: hidden;
    }

    /* Animated Background */
    .bg-animation {
        position: fixed;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        z-index: 0;
        overflow: hidden;
    }

    .bg-animation span {
        position: absolute;
        width: 2px;
        height: 2px;
        background: var(--accent);
        box-shadow: 0 0 10px var(--accent);
        border-radius: 50%;
        animation: float 15s infinite;
    }

    @keyframes float {
        0%, 100% { transform: translateY(0) translateX(0); opacity: 0; }
        10% { opacity: 1; }
        90% { opacity: 1; }
        100% { transform: translateY(-100vh) translateX(100px); opacity: 0; }
    }

    /* Navigation */
    nav {
        position: fixed;
        top: 0;
        width: 100%;
        /* Adjusted background for better visibility/blur */
        background: rgba(10, 14, 39, 0.9); 
        backdrop-filter: blur(10px);
        padding: 1rem 5%; /* Slight adjustment */
        z-index: 1000;
        border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    }

    nav ul {
        display: flex;
        justify-content: center;
        gap: 2rem;
        list-style: none;
        /* Removed flex-wrap: wrap to force a single line */
        /* flex-wrap: wrap; */ 
    }

    nav a {
        color: var(--light);
        text-decoration: none;
        font-weight: 500;
        transition: color 0.3s;
        position: relative;
        /* Ensure text stays visible on small screens */
        white-space: nowrap; 
    }

    nav a::after {
        content: '';
        position: absolute;
        bottom: -5px;
        left: 0;
        width: 0;
        height: 2px;
        background: linear-gradient(90deg, var(--primary), var(--secondary));
        transition: width 0.3s;
    }

    nav a:hover::after {
        width: 100%;
    }

    /* Hero Section */
    .hero {
        position: relative;
        /* Reduced min-height slightly and adjusted for nav bar */
        min-height: calc(100vh - 80px); 
        padding-top: 80px; /* Added padding to start below the fixed nav */
        display: flex;
        align-items: center;
        justify-content: center;
        text-align: center;
        padding-bottom: 2rem; /* Ensure there's padding on the bottom */
        z-index: 1;
    }
    
    .hero-content {
        animation: fadeInUp 1s ease-out;
    }

    .profile-img {
        width: 180px;
        height: 180px;
        border-radius: 50%;
        border: 4px solid var(--primary);
        box-shadow: 0 0 40px rgba(13, 110, 253, 0.5);
        margin-bottom: 2rem;
        animation: float-img 3s ease-in-out infinite;
    }

    @keyframes float-img {
        0%, 100% { transform: translateY(0); }
        50% { transform: translateY(-20px); }
    }

    h1 {
        font-size: 3.5rem;
        background: linear-gradient(135deg, var(--primary), var(--secondary));
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        margin-bottom: 1rem;
    }

    .subtitle {
        font-size: 1.5rem;
        color: var(--accent);
        margin-bottom: 2rem;
    }

    .social-links {
        display: flex;
        gap: 1rem;
        justify-content: center;
        flex-wrap: wrap;
        margin-top: 2rem;
    }

    .social-btn {
        padding: 0.8rem 2rem;
        border-radius: 50px;
        text-decoration: none;
        color: white;
        font-weight: 600;
        transition: transform 0.3s, box-shadow 0.3s;
        display: inline-block;
    }

    .social-btn:hover {
        transform: translateY(-3px);
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
    }

    .linkedin { background: linear-gradient(135deg, #0A66C2, #004182); }
    .github { background: linear-gradient(135deg, #333, #000); }
    .email { background: linear-gradient(135deg, #D14836, #8B0000); }

    /* Section Container */
    section {
        position: relative;
        max-width: 1200px;
        margin: 5rem auto;
        padding: 2rem;
        z-index: 1;
    }
    
    /* FIX: Added specific padding to the first section to clear the fixed nav bar */
    #about {
        padding-top: 8rem; 
        margin-top: 0;
    }


    .section-title {
        font-size: 2.5rem;
        text-align: center;
        margin-bottom: 3rem;
        background: linear-gradient(135deg, var(--primary), var(--secondary));
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    /* Cards */
    .card {
        background: rgba(255, 255, 255, 0.05);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 20px;
        padding: 2rem;
        margin-bottom: 2rem;
        transition: transform 0.3s, box-shadow 0.3s;
    }

    .card:hover {
        transform: translateY(-10px);
        box-shadow: 0 20px 40px rgba(13, 110, 253, 0.3);
    }

    /* Skills Grid */
    .skills-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
        gap: 2rem;
        text-align: center;
    }

    .skill-item {
        padding: 1.5rem;
        background: rgba(255, 255, 255, 0.05);
        border-radius: 15px;
        transition: all 0.3s;
    }

    .skill-item:hover {
        background: rgba(13, 110, 253, 0.2);
        transform: scale(1.1);
    }

    .skill-icon {
        font-size: 3rem;
        margin-bottom: 0.5rem;
    }

    /* Projects Grid */
    .projects-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 2rem;
    }

    .project-card {
        background: linear-gradient(135deg, rgba(13, 110, 253, 0.1), rgba(111, 66, 193, 0.1));
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 20px;
        padding: 2rem;
        transition: transform 0.3s;
    }

    .project-card:hover {
        transform: translateY(-10px);
        box-shadow: 0 20px 40px rgba(111, 66, 193, 0.3);
    }

    .project-card h3 {
        color: var(--accent);
        margin-bottom: 1rem;
    }

    .tech-stack {
        display: flex;
        flex-wrap: wrap;
        gap: 0.5rem;
        margin-top: 1rem;
    }

    .tech-tag {
        padding: 0.3rem 0.8rem;
        background: rgba(13, 110, 253, 0.3);
        border-radius: 20px;
        font-size: 0.85rem;
    }

    /* Timeline */
    .timeline {
        position: relative;
        padding-left: 2rem;
    }

    .timeline::before {
        content: '';
        position: absolute;
        left: 0;
        top: 0;
        height: 100%;
        width: 2px;
        background: linear-gradient(180deg, var(--primary), var(--secondary));
    }

    .timeline-item {
        margin-bottom: 2rem;
        position: relative;
    }

    .timeline-item::before {
        content: '';
        position: absolute;
        left: -2.5rem;
        top: 0;
        width: 12px;
        height: 12px;
        border-radius: 50%;
        background: var(--accent);
        box-shadow: 0 0 20px var(--accent);
    }

    /* Achievement Badges */
    .achievements-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 1.5rem;
    }

    .achievement-badge {
        background: linear-gradient(135deg, rgba(13, 110, 253, 0.2), rgba(111, 66, 193, 0.2));
        padding: 1.5rem;
        border-radius: 15px;
        text-align: center;
        border: 1px solid rgba(255, 255, 255, 0.1);
    }

    .badge-icon {
        font-size: 3rem;
        margin-bottom: 1rem;
    }

    /* Table */
    table {
        width: 100%;
        border-collapse: collapse;
        margin: 2rem 0;
    }

    th, td {
        padding: 1rem;
        text-align: left;
        border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    }

    th {
        background: rgba(13, 110, 253, 0.2);
        color: var(--accent);
    }

    /* Footer */
    footer {
        text-align: center;
        padding: 3rem 2rem;
        background: rgba(0, 0, 0, 0.3);
        margin-top: 5rem;
    }

    @keyframes fadeInUp {
        from {
            opacity: 0;
            transform: translateY(30px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    /* Responsive */
    @media (max-width: 768px) {
        h1 { font-size: 2rem; }
        .subtitle { font-size: 1.2rem; }
        .section-title { font-size: 2rem; }
        
        /* Allow navigation to wrap on smaller screens if necessary */
        nav ul { 
            gap: 1rem;
            flex-wrap: wrap; /* Re-enabled for small screens */
            padding-bottom: 0.5rem;
        }

        /* Adjust padding for small screens */
        #about {
            padding-top: 10rem; /* Increased padding for the wrapping nav */
        }
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
