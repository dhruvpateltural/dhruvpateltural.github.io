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
            --bg-1:#eaf4ff;
            --bg-2:#d6ebff;
            --primary:#0b63f6;
            --primary-2:#094bb5;
            --accent:#6fb3ff;
            --glass-bg:rgba(255,255,255,0.10);
            --glass-bg-2:rgba(11,99,246,0.06);
            --muted:#4b6b86;
            --shadow:0 10px 30px rgba(11,99,246,0.12);
            --glass-shadow:0 6px 20px rgba(7,40,90,0.08);
            --glass-radius:14px;
            --text:#02213b;
        }

        *{box-sizing:border-box;margin:0;padding:0;scroll-behavior:smooth}
        html,body{height:100%}
        body{
            font-family:"Inter",system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
            background:linear-gradient(180deg,var(--bg-1),var(--bg-2));
            color:var(--text);
            -webkit-font-smoothing:antialiased;
            -moz-osx-font-smoothing:grayscale;
            line-height:1.5;
            padding-bottom:60px;
        }

        a{color:var(--primary);text-decoration:none}

        h1,h2,h3{color:var(--text);margin-bottom:8px}
        h2{font-size:1.9rem;font-weight:800;display:flex;align-items:center;gap:.6rem}
        h3{font-size:1.05rem}

        main{
            max-width:1100px;
            margin:0 auto;
            padding:0 20px 40px;
        }

        /* NAVBAR */
        header.site-header{
            position:sticky;
            top:18px;
            z-index:120;
            margin:12px auto 0;
            max-width:980px;
        }

        nav.main-nav{
            width:100%;
            display:flex;
            justify-content:center;
            align-items:center;
            padding:10px 20px;
            backdrop-filter:blur(6px) saturate(140%);
            background:linear-gradient(180deg,rgba(255,255,255,0.55),rgba(255,255,255,0.35));
            border:1px solid rgba(255,255,255,0.6);
            box-shadow:var(--glass-shadow);
            border-radius:40px;
        }

        ul.nav-links{
            display:flex;
            gap:10px;
            align-items:center;
            list-style:none;
        }

        ul.nav-links a{
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

        ul.nav-links a:hover{
            background:linear-gradient(90deg,rgba(11,99,246,0.12),rgba(9,75,181,0.08));
            transform:translateY(-3px);
            box-shadow:0 6px 18px rgba(11,99,246,0.08);
        }

        /* HERO */
        section.hero{
            margin:30px auto;
            max-width:1100px;
            position:relative;
            padding:48px;
            display:flex;
            gap:28px;
            align-items:center;
            border-radius:18px;
            background:linear-gradient(135deg,rgba(11,99,246,0.95),rgba(9,75,181,0.92));
            color:white;
            box-shadow:var(--shadow);
            overflow:hidden;
        }

        section.hero::before{
            content:"";
            position:absolute;
            right:-120px;
            top:-80px;
            width:380px;
            height:380px;
            background:radial-gradient(circle at 30% 30%,rgba(96,165,250,0.18),rgba(11,99,246,0.06));
            transform:rotate(25deg);
            filter:blur(30px);
            opacity:0.85;
        }

        section.hero .hero-left{
            display:flex;
            align-items:center;
            gap:18px;
            z-index:2;
            flex:1;
        }

        figure.avatar{
            width:130px;
            height:130px;
            border-radius:22px;
            overflow:hidden;
            border:4px solid rgba(255,255,255,0.14);
            box-shadow:0 10px 30px rgba(3,12,40,0.3);
            flex-shrink:0;
            margin:0;
        }

        figure.avatar img{
            width:100%;
            height:100%;
            object-fit:cover;
            display:block;
        }

        .hero-info h1{
            font-size:1.8rem;
            margin-bottom:6px;
            display:flex;
            align-items:center;
            gap:10px;
        }

        .hero-info h3{
            opacity:0.95;
            font-weight:500;
            color:rgba(255,255,255,0.92);
            font-size:1rem;
            margin-bottom:14px;
        }

        .hero-ctas{
            display:flex;
            gap:12px;
            align-items:center;
            margin-top:6px;
        }

        .btn{
            padding:10px 16px;
            border-radius:10px;
            font-weight:700;
            font-size:14px;
            border:none;
            cursor:pointer;
            display:inline-flex;
            gap:10px;
            align-items:center;
            transition:all .18s ease;
        }

        .btn-primary{
            background:linear-gradient(90deg,var(--accent),#2b6cf6);
            color:white;
            box-shadow:0 8px 22px rgba(11,99,246,0.24);
        }

        .btn-outline{
            background:transparent;
            color:white;
            border:1px solid rgba(255,255,255,0.18);
        }

        .btn:hover{transform:translateY(-4px)}

        aside.hero-right{
            margin-left:auto;
            text-align:right;
            z-index:2;
        }

        .availability{
            background:rgba(255,255,255,0.06);
            padding:10px 14px;
            border-radius:12px;
            border:1px solid rgba(255,255,255,0.08);
            display:inline-block;
        }

        .availability-title{
            font-weight:700;
            font-size:14px;
        }

        .availability-sub{
            font-size:13px;
            opacity:0.95;
        }

        ul.socials{
            margin-top:16px;
            display:flex;
            gap:12px;
            align-items:center;
            list-style:none;
            justify-content:flex-end;
        }

        ul.socials a{
            width:38px;
            height:38px;
            border-radius:10px;
            display:inline-flex;
            align-items:center;
            justify-content:center;
            background:rgba(255,255,255,0.12);
            color:white;
            font-size:16px;
            transition:all .15s linear;
        }

        ul.socials a:hover{
            transform:translateY(-3px);
            background:rgba(255,255,255,0.18);
        }

        /* Sections / cards */
        section.block{
            margin:45px auto 0;
            max-width:1100px;
        }

        .section-card{
            background:linear-gradient(180deg,rgba(255,255,255,0.82),rgba(255,255,255,0.72));
            border-radius:var(--glass-radius);
            padding:20px;
            box-shadow:var(--glass-shadow);
            border:1px solid rgba(255,255,255,0.6);
            transition:transform .18s ease,box-shadow .18s ease;
            margin-top:12px;
        }

        .section-card:hover{
            transform:translateY(-6px);
            box-shadow:0 18px 40px rgba(7,40,90,0.08);
        }

        p{color:var(--muted);margin-top:8px}
        ul{padding-left:18px;margin-top:8px}
        li{margin-bottom:8px;color:var(--muted);font-weight:500}

        /* Skills */
        section.skills{
            text-align:center;
        }

        section.skills img{
            width:80%;
            max-width:520px;
            border-radius:10px;
        }

        /* Projects grid */
        section.projects-list{
            display:grid;
            grid-template-columns:repeat(2,1fr);
            gap:18px;
            margin-top:12px;
        }

        article.project-card{
            padding:18px;
            border-radius:12px;
            background:linear-gradient(180deg,#ffffff,#f7fbff);
            border:1px solid rgba(9,75,181,0.06);
            box-shadow:0 8px 18px rgba(9,75,181,0.04);
        }

        article.project-card h3{
            display:flex;
            align-items:center;
            gap:10px;
            font-size:1.05rem;
            margin-bottom:8px;
        }

        .meta{
            font-size:13px;
            color:var(--muted);
            margin-bottom:8px;
        }

        /* Education */
        section.education-grid{
            margin-top:12px;
            display:grid;
            grid-template-columns:repeat(2,1fr);
            gap:16px;
        }

        /* Animations */
        .fade-up{animation:fadeUp .6s ease both}
        @keyframes fadeUp{
            from{opacity:0;transform:translateY(10px)}
            to{opacity:1;transform:none}
        }

        /* Responsive */
        @media (max-width:900px){
            section.hero{
                flex-direction:column;
                align-items:flex-start;
                padding:26px;
            }
            section.hero::before{display:none}
            section.projects-list{grid-template-columns:1fr}
            nav.main-nav{margin:10px 12px}
            ul.nav-links{overflow:auto;padding:6px 2px}
        }

        @media (max-width:480px){
            figure.avatar{width:100px;height:100px}
            .hero-info h1{font-size:1.3rem}
            .hero-info h3{font-size:.94rem}
            main{padding:0 14px 40px}
            ul.nav-links a{padding:8px}
        }
    </style>
</head>

<body>
    <header class="site-header" aria-label="Primary navigation">
        <nav class="main-nav">
            <ul class="nav-links">
                <li><a href="#about"><i class="fa-solid fa-user"></i> About</a></li>
                <li><a href="#skills"><i class="fa-solid fa-code"></i> Skills</a></li>
                <li><a href="#internship"><i class="fa-solid fa-briefcase"></i> Internship</a></li>
                <li><a href="#projects"><i class="fa-solid fa-diagram-project"></i> Projects</a></li>
                <li><a href="#education"><i class="fa-solid fa-graduation-cap"></i> Education</a></li>
                <li><a href="#certifications"><i class="fa-solid fa-certificate"></i> Certifications</a></li>
                <li><a href="#achievements"><i class="fa-solid fa-trophy"></i> Achievements</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <!-- HERO -->
        <section class="hero fade-up" id="home" aria-label="Intro">
            <section class="hero-left">
                <figure class="avatar">
                    <img src="https://avatars.githubusercontent.com/u/0?v=4" alt="Portrait of Dhruv Manohar Patel">
                </figure>
                <section class="hero-info">
                    <h1><i class="fa-solid fa-user"></i> Dhruv Manohar Patel</h1>
                    <h3>Full Stack .NET Developer • Backend Specialist • MCA Graduate</h3>
                    <section class="hero-ctas" aria-label="Primary actions">
                        <a class="btn btn-primary" href="#projects">
                            <i class="fa-solid fa-rocket"></i> View Projects
                        </a>
                        <a class="btn btn-outline" href="mailto:dhruvpateltural@gmail.com">
                            <i class="fa-solid fa-envelope"></i> Contact
                        </a>
                    </section>
                </section>
            </section>

            <aside class="hero-right" aria-label="Availability and social links">
                <section class="availability">
                    <p class="availability-title">Open to work</p>
                    <p class="availability-sub">Backend &amp; .NET Roles • Remote/Hybrid</p>
                </section>

                <ul class="socials">
                    <li>
                        <a href="https://linkedin.com/in/dhruvpateltural" aria-label="LinkedIn">
                            <i class="fab fa-linkedin"></i>
                        </a>
                    </li>
                    <li>
                        <a href="https://github.com/dhruvpateltural" aria-label="GitHub">
                            <i class="fab fa-github"></i>
                        </a>
                    </li>
                    <li>
                        <a href="mailto:dhruvpateltural@gmail.com" aria-label="Email">
                            <i class="fa-solid fa-envelope"></i>
                        </a>
                    </li>
                </ul>
            </aside>
        </section>

        <!-- ABOUT -->
        <section id="about" class="block fade-up" aria-labelledby="about-heading">
            <h2 id="about-heading"><i class="fa-solid fa-user"></i> About Me</h2>
            <section class="section-card">
                <p>
                    MCA graduate with <strong>full-stack development</strong> experience using
                    <strong>C#, ASP.NET, SQL Server &amp; Entity Framework</strong>. I build
                    <strong>secure, scalable backend systems</strong>, optimize databases,
                    and work efficiently in <strong>Agile SDLC environments</strong>.
                </p>
            </section>
        </section>

        <!-- SKILLS -->
        <section id="skills" class="block skills fade-up" aria-labelledby="skills-heading">
            <h2 id="skills-heading"><i class="fa-solid fa-code"></i> Tech Stack</h2>
            <section class="section-card">
                <figure>
                    <img src="https://skillicons.dev/icons?i=cs,dotnet,java,html,css,js,git,github,visualstudio,mysql"
                         alt="Icons representing C#, .NET, Java, HTML, CSS, JavaScript, Git, GitHub, Visual Studio, and MySQL">
                </figure>
                <p>C#, .NET, SQL Server, EF, ASP.NET, WinForms, HTML/CSS/JS and tooling (Git, Visual Studio)</p>
            </section>
        </section>

        <!-- INTERNSHIP -->
        <section id="internship" class="block fade-up" aria-labelledby="internship-heading">
            <h2 id="internship-heading"><i class="fa-solid fa-briefcase"></i> Internship</h2>
            <article class="section-card">
                <header>
                    <h3><i class="fa-solid fa-building"></i> Software Development Intern — Aaryak Solutions</h3>
                    <p class="meta"><strong>Jan 2025 – Jun 2025</strong></p>
                </header>
                <ul>
                    <li>Developed 10+ backend modules</li>
                    <li>Improved SQL performance by 20–30%</li>
                    <li>Implemented RBAC-based security</li>
                    <li>Collaborated in Agile SDLC</li>
                </ul>
            </article>
        </section>

        <!-- PROJECTS -->
        <section id="projects" class="block fade-up" aria-labelledby="projects-heading">
            <h2 id="projects-heading"><i class="fa-solid fa-diagram-project"></i> Projects</h2>

            <section class="projects-list" aria-label="Project list">
                <article class="project-card">
                    <h3><i class="fa-solid fa-utensils"></i> Restaurant Management System</h3>
                    <p class="meta"><strong>Tech:</strong> C#, ASP.NET, SQL Server, EF, HTML, CSS</p>
                    <ul>
                        <li>Billing, orders and inventory automation</li>
                        <li>Secure role-based authentication</li>
                        <li>Optimized backend APIs</li>
                    </ul>
                </article>

                <article class="project-card">
                    <h3><i class="fa-solid fa-gears"></i> Hardware Shop Management System</h3>
                    <p class="meta"><strong>Tech:</strong> WinForms, C#, SQL Server, EF</p>
                    <ul>
                        <li>Sales and inventory automation</li>
                        <li>ORM-based reliable data handling</li>
                    </ul>
                </article>
            </section>
        </section>

        <!-- EDUCATION -->
        <section id="education" class="block fade-up" aria-labelledby="education-heading">
            <h2 id="education-heading"><i class="fa-solid fa-graduation-cap"></i> Education</h2>

            <section class="education-grid" aria-label="Education details">
                <article class="section-card">
                    <h3>MCA — Finolex Academy</h3>
                    <p class="meta">2025</p>
                    <strong>CGPA: 8.4</strong>
                </article>

                <article class="section-card">
                    <h3>B.Com — Gogate Jogalekar College</h3>
                    <p class="meta">2023</p>
                    <strong>CGPA: 8.78</strong>
                </article>
            </section>
        </section>

        <!-- CERTIFICATIONS -->
        <section id="certifications" class="block fade-up" aria-labelledby="certifications-heading">
            <h2 id="certifications-heading"><i class="fa-solid fa-certificate"></i> Certifications</h2>
            <section class="section-card">
                <ul>
                    <li>Java Programming Fundamentals — SpringBoard</li>
                    <li>Cyber Security &amp; Privacy Fundamentals — NPTEL</li>
                    <li>Web Development Fundamentals — IBM</li>
                </ul>
            </section>
        </section>

        <!-- ACHIEVEMENTS -->
        <section id="achievements" class="block fade-up" aria-labelledby="achievements-heading">
            <h2 id="achievements-heading"><i class="fa-solid fa-trophy"></i> Achievements</h2>

            <section class="section-card">
                <ul>
                    <li>Marketing Lead — Excellentia 2K25</li>
                    <li>Photography &amp; Videography Coordinator — Finolex MCA Dept</li>
                </ul>
            </section>

            <h3 style="margin-top:18px">Core Strengths</h3>
            <section class="section-card" aria-label="Core strengths">
                <ul>
                    <li>Problem solving</li>
                    <li>Agile collaboration</li>
                    <li>Analytical thinking</li>
                    <li>Time management</li>
                </ul>
            </section>
        </section>
    </main>

    <footer>
        <p>
            ⭐ If you like my work, consider starring my repositories and connecting with me.
        </p>
        <p>
            © 2025 Dhruv Manohar Patel
        </p>
    </footer>
</body>
</html>
