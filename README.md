<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Dhruv Manohar Patel | Full Stack .NET Developer</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Dhruv Manohar Patel - Full Stack .NET Developer, Backend Specialist, MCA Graduate" />
    <link rel="icon" href="https://avatars.githubusercontent.com/u/0?v=4" />

    <!-- Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

    <!-- Modern font -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

    <style>
        :root{
            /* Blue / Liquid glass palette */
            --bg-1: #eaf4ff;               /* very light blue */
            --bg-2: #d6ebff;               /* light blue gradient stop */
            --primary: #0b63f6;            /* vivid blue */
            --primary-2: #094bb5;          /* darker blue */
            --accent: #6fb3ff;             /* soft accent blue */
            --glass-bg: rgba(255,255,255,0.10); /* translucent base for glass */
            --glass-bg-2: rgba(11,99,246,0.06); /* bluish translucent overlay */
            --muted: #4b6b86;
            --shadow: 0 10px 30px rgba(11,99,246,0.12);
            --glass-shadow: 0 6px 20px rgba(7,40,90,0.08);
            --glass-radius: 14px;
        }

        *{box-sizing:border-box;margin:0;padding:0;scroll-behavior:smooth}
        html,body{height:100%}
        body{
            font-family:"Inter",system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
            background: linear-gradient(180deg, var(--bg-1), var(--bg-2));
            color:var(--text);
            -webkit-font-smoothing:antialiased;
            -moz-osx-font-smoothing:grayscale;
            line-height:1.5;
            padding-bottom:60px;
        }

        a{color:var(--primary);text-decoration:none}
        .section{max-width:1100px;margin:45px auto;padding:0 20px}
        h1,h2,h3{color:var(--text);margin-bottom:8px}
        h2{font-size:1.9rem;font-weight:800;display:flex;align-items:center;gap:.6rem}
        h3{font-size:1.05rem}

        /* Top decorative waves */
        .page-wrap{
            position:relative;
            overflow:visible;
        }

        /* NAVBAR */
        .navbar{
            width:100%;
            position:sticky;
            top:18px;
            z-index:120;
            display:flex;
            justify-content:center;
            align-items:center;
            padding:10px 20px;
            backdrop-filter: blur(6px) saturate(140%);
            background: linear-gradient(180deg, rgba(255,255,255,0.55), rgba(255,255,255,0.35));
            border:1px solid rgba(255,255,255,0.6);
            box-shadow: var(--glass-shadow);
            border-radius:40px;
            margin:12px auto;
            max-width:980px;
        }

        .nav-links{
            display:flex;
            gap:10px;
            align-items:center;
        }

        .nav-links a{
            display:inline-flex;
            gap:8px;
            align-items:center;
            padding:8px 12px;
            border-radius:999px;
            color:var(--primary-2);
            font-weight:600;
            transition:all .18s ease;
            font-size:14px;
        }

        .nav-links a:hover{
            background:linear-gradient(90deg, rgba(11,99,246,0.12), rgba(9,75,181,0.08));
            transform:translateY(-3px);
            box-shadow:0 6px 18px rgba(11,99,246,0.08);
        }

        /* HERO */
        .hero{
            margin:30px auto;
            max-width:1100px;
            position:relative;
            padding:48px;
            display:flex;
            gap:28px;
            align-items:center;
            border-radius:18px;
            background:linear-gradient(135deg, rgba(11,99,246,0.95), rgba(9,75,181,0.92));
            color:white;
            box-shadow:var(--shadow);
            overflow:hidden;
        }

        .hero::before{
            content:"";
            position:absolute;
            right:-120px;
            top:-80px;
            width:380px;
            height:380px;
            background:radial-gradient(circle at 30% 30%, rgba(96,165,250,0.18), rgba(11,99,246,0.06));
            transform:rotate(25deg);
            filter: blur(30px);
            opacity:0.85;
        }

        .hero-left{
            display:flex;
            align-items:center;
            gap:18px;
            z-index:2;
            flex:1;
        }

        .avatar{
            width:130px;
            height:130px;
            border-radius:22px;
            overflow:hidden;
            border:4px solid rgba(255,255,255,0.14);
            box-shadow:0 10px 30px rgba(3,12,40,0.3);
            flex-shrink:0;
        }

        .avatar img{width:100%;height:100%;object-fit:cover;display:block}

        .hero-info h1{font-size:1.8rem;margin-bottom:6px;display:flex;align-items:center;gap:10px}
        .hero-info h3{opacity:0.95;font-weight:500;color:rgba(255,255,255,0.92);font-size:1rem;margin-bottom:14px}

        .hero-ctas{display:flex;gap:12px;align-items:center}
        .btn{
            padding:10px 16px;border-radius:10px;font-weight:700;font-size:14px;border:none;cursor:pointer;
            display:inline-flex;gap:10px;align-items:center;transition:all .18s ease;
        }

        .btn-primary{
            background:linear-gradient(90deg,var(--accent),#2b6cf6);
            color:white;
            box-shadow:0 8px 22px rgba(11,99,246,0.24);
        }

        .btn-outline{
            background:transparent;color:white;border:1px solid rgba(255,255,255,0.18);
        }

        .btn:hover{transform:translateY(-4px)}
        .socials{display:flex;gap:12px;align-items:center}

        .socials a{
            width:38px;height:38px;border-radius:10px;display:inline-flex;align-items:center;justify-content:center;
            background:rgba(255,255,255,0.12);color:white;font-size:16px;transition:all .15s linear;
        }

        .socials a:hover{transform:translateY(-3px);background:rgba(255,255,255,0.18)}

        /* SECTIONS - Glass cards */
        .section-card{
            background: linear-gradient(180deg, rgba(255,255,255,0.82), rgba(255,255,255,0.72));
            border-radius: var(--glass-radius);
            padding:20px;
            box-shadow: var(--glass-shadow);
            border:1px solid var(--glass-border);
            transition:transform .18s ease, box-shadow .18s ease;
        }

        .section-card:hover{transform:translateY(-6px);box-shadow:0 18px 40px rgba(7,40,90,0.08)}

        /* Skills image */
        .skills .section-card{display:flex;flex-direction:column;align-items:center;gap:12px}
        .skills img{width:80%;max-width:520px;border-radius:10px}

        /* Lists and typography */
        ul{padding-left:18px;margin-top:8px}
        li{margin-bottom:8px;color:var(--muted);font-weight:500}
        p{color:var(--muted);Margin-top:8px}

        /* Projects grid */
        .projects-grid{
            display:grid;
            grid-template-columns:repeat(2,1fr);
            gap:18px;margin-top:12px;
        }

        .project-card{
            padding:18px;border-radius:12px;background:linear-gradient(180deg,#ffffff,#f7fbff);
            border:1px solid rgba(9,75,181,0.06);
            box-shadow:0 8px 18px rgba(9,75,181,0.04);
        }

        .project-card h3{display:flex;align-items:center;gap:10px;font-size:1.05rem;margin-bottom:8px}
        .meta{font-size:13px;color:var(--muted);margin-bottom:8px}

        /* Footer */
        footer{
            margin-top:40px;
            text-align:center;
            font-size:14px;
            color:var(--muted);
            padding:28px 16px;
            max-width:1100px;margin-left:auto;margin-right:auto;
        }

        /* Animations */
        .fade-up{animation:fadeUp .6s ease both}
        @keyframes fadeUp{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}

        /* Responsive */
        @media (max-width:900px){
            .hero{flex-direction:column;align-items:flex-start;padding:26px}
            .hero::before{display:none}
            .projects-grid{grid-template-columns:1fr}
            .nav-links{overflow:auto;padding:6px 2px}
            .navbar{margin:10px 12px}
        }

        @media (max-width:480px){
            .avatar{width:100px;height:100px}
            .hero-info h1{font-size:1.3rem}
            .hero-info h3{font-size:.94rem}
            .section{padding:0 14px}
            .nav-links a{padding:8px}
        }
    </style>
</head>
<body>
    <div class="page-wrap">
        <!-- NAVBAR -->
        <div class="navbar fade-up" role="navigation" aria-label="Primary">
            <nav class="nav-links">
                <a href="#about"><i class="fa-solid fa-user"></i> About</a>
                <a href="#skills"><i class="fa-solid fa-code"></i> Skills</a>
                <a href="#internship"><i class="fa-solid fa-briefcase"></i> Internship</a>
                <a href="#projects"><i class="fa-solid fa-diagram-project"></i> Projects</a>
                <a href="#education"><i class="fa-solid fa-graduation-cap"></i> Education</a>
                <a href="#certifications"><i class="fa-solid fa-certificate"></i> Certifications</a>
                <a href="#achievements"><i class="fa-solid fa-trophy"></i> Achievements</a>
            </nav>
        </div>

        <!-- HERO -->
        <header class="hero fade-up" id="home" role="banner">
            <div class="hero-left">
                <div class="avatar">
                    <img src="https://avatars.githubusercontent.com/u/0?v=4" alt="Dhruv avatar">
                </div>
                <div class="hero-info">
                    <h1><i class="fa-solid fa-user"></i> Dhruv Manohar Patel</h1>
                    <h3>Full Stack .NET Developer • Backend Specialist • MCA Graduate</h3>
                    <div class="hero-ctas">
                        <a class="btn btn-primary" href="#projects"><i class="fa-solid fa-rocket"></i> View Projects</a>
                        <a class="btn btn-outline" href="mailto:dhruvpateltural@gmail.com"><i class="fa-solid fa-envelope"></i> Contact</a>
                    </div>
                </div>
            </div>

            <div style="margin-left:auto;text-align:right;z-index:2">
                <div style="background:rgba(255,255,255,0.06);padding:10px 14px;border-radius:12px;border:1px solid rgba(255,255,255,0.08);display:inline-block">
                    <div style="font-weight:700;font-size:14px">Open to work</div>
                    <div style="font-size:13px;opacity:0.95">Backend & .NET Roles • Remote/Hybrid</div>
                </div>

                <div style="margin-top:16px" class="socials">
                    <a href="https://linkedin.com/in/dhruvpateltural" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
                    <a href="https://github.com/dhruvpateltural" aria-label="GitHub"><i class="fab fa-github"></i></a>
                    <a href="mailto:dhruvpateltural@gmail.com" aria-label="Email"><i class="fa-solid fa-envelope"></i></a>
                </div>
            </div>
        </header>

        <!-- ABOUT -->
        <div id="about" class="section fade-up" aria-labelledby="about-heading" role="region"></div>
            <h2 id="about-heading"><i class="fa-solid fa-user"></i> About Me</h2>
            <div class="section-card" style="margin-top:12px">
                <p style="font-weight:600;color:var(--text)"></p>
                    MCA graduate with <strong>full-stack development</strong> experience using
                    <strong>C#, ASP.NET, SQL Server & Entity Framework</strong>. I build
                    <strong>secure, scalable backend systems</strong>, optimize databases,
                    and work efficiently in <strong>Agile SDLC environments</strong>.
                </p>
            </div>
        </div>

        <!-- SKILLS -->
        <div id="skills" class="skills section fade-up" aria-labelledby="skills-heading" role="region"></div>
            <h2 id="skills-heading"><i class="fa-solid fa-code"></i> Tech Stack</h2>
            <div class="section-card" style="margin-top:12px;text-align:center">
                <img src="https://skillicons.dev/icons?i=cs,dotnet,java,html,css,js,git,github,visualstudio,mysql" alt="tech stack icons">
                <p style="margin-top:10px;color:var(--muted)">C#, .NET, SQL Server, EF, ASP.NET, WinForms, HTML/CSS/JS and tooling (Git, VS)</p>
            </div>
        

        <!-- INTERNSHIP -->
        <div id="internship" class="section fade-up" aria-labelledby="internship-heading" role="region"></div>
            <h2 id="internship-heading"><i class="fa-solid fa-briefcase"></i> Internship</h2>
            <div class="section-card" style="margin-top:12px">
                <h3><i class="fa-solid fa-building"></i> Software Development Intern — Aaryak Solutions</h3>
                <p class="meta"><strong>Jan 2025 – Jun 2025</strong></p>
                <ul>
                    <li>Developed 10+ backend modules</li>
                    <li>Improved SQL performance by 20–30%</li>
                    <li>Implemented RBAC-based security</li>
                    <li>Collaborated in Agile SDLC</li>
                </ul>
            </div>
   

        <!-- PROJECTS -->
        <div id="projects" class="section fade-up" aria-labelledby="projects-heading" role="region"></div>
            <h2 id="projects-heading"><i class="fa-solid fa-diagram-project"></i> Projects</h2>

            <div class="projects-grid" style="margin-top:12px">
                <div class="project-card">
                    <h3><i class="fa-solid fa-utensils"></i> Restaurant Management System</h3>
                    <div class="meta"><strong>Tech:</strong> C#, ASP.NET, SQL Server, EF, HTML, CSS</div>
                    <ul>
                        <li>Billing, Orders & Inventory Automation</li>
                        <li>Secure Role-Based Authentication</li>
                        <li>Optimized Backend APIs</li>
                    </ul>
                </div>

                <div class="project-card">
                    <h3><i class="fa-solid fa-gears"></i> Hardware Shop Management System</h3>
                    <div class="meta"><strong>Tech:</strong> WinForms, C#, SQL Server, EF</div>
                    <ul>
                        <li>Sales & Inventory Automation</li>
                        <li>ORM-based Reliable Data Handling</li>
                    </ul>
                </div>
            </div>
        

        <!-- EDUCATION -->
        <div id="education" class="section fade-up" aria-labelledby="education-heading" role="region">
            <h2 id="education-heading"><i class="fa-solid fa-graduation-cap"></i> Education</h2>

            <div style="margin-top:12px;display:grid;grid-template-columns:repeat(2,1fr);gap:16px">
                <div class="section-card">
                    <h3>MCA — Finolex Academy</h3>
                    <p class="meta">2025</p>
                    <strong>CGPA: 8.4</strong>
                </div>

                <div class="section-card">
                    <h3>B.Com — Gogate Jogalekar College</h3>
                    <p class="meta">2023</p>
                    <strong>CGPA: 8.78</strong>
                </div>
            </div>
        </div>

        <!-- CERTIFICATIONS -->
        <div id="certifications" class="section fade-up" aria-labelledby="certifications-heading" role="region">
            <h2 id="certifications-heading"><i class="fa-solid fa-certificate"></i> Certifications</h2>
            <div class="section-card" style="margin-top:12px"></div>
                <ul>
                    <li>Java Programming Fundamentals — SpringBoard</li>
                    <li>Cyber Security & Privacy Fundamentals — NPTEL</li>
                    <li>Web Development Fundamentals — IBM</li>
                </ul>
            </div>
       

        <!-- ACHIEVEMENTS -->
        <div id="achievements" class="section fade-up" aria-labelledby="achievements-heading" role="region">
            <h2 id="achievements-heading"><i class="fa-solid fa-trophy"></i> Achievements</h2>

            <div class="section-card" style="margin-top:12px">
                <ul>
                    <li>Marketing Lead — Excellentia 2K25</li>
                    <li>Photography & Videography Coordinator — Finolex MCA Dept</li>
                </ul>
            </div>

            <h3 style="margin-top:18px">Core Strengths</h3>
            <div class="section-card" style="margin-top:10px">
                <ul>
                    <li>Problem Solving</li>
                    <li>Agile Collaboration</li>
                    <li>Analytical Thinking</li>
                    <li>Time Management</li>
                </ul>
            </div>
        </div>

        <!-- FOOTER -->
        <footer>
            ⭐ If you like my work, consider starring my repositories and connecting with me.
            <br><br>
            © 2025 Dhruv Manohar Patel
        </footer>
    </div>
</body>
</html>
