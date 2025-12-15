<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Dhruv Manohar Patel | Full Stack .NET Developer</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Dhruv Manohar Patel - Full Stack .NET Developer, Backend Specialist, MCA Graduate" />
    <link rel="icon" href="https://avatars.githubusercontent.com/u/0?v=4" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

    <style>
        :root{
            --bg-1:#0a0e27;
            --bg-2:#151937;
            --primary:#6366f1;
            --primary-light:#818cf8;
            --accent:#a78bfa;
            --text:#e2e8f0;
            --text-muted:#94a3b8;
            --card-bg:rgba(30, 41, 59, 0.5);
            --glass-border:rgba(148, 163, 184, 0.1);
            --shadow:0 20px 50px rgba(0, 0, 0, 0.3);
            --glow:0 0 30px rgba(99, 102, 241, 0.3);
        }

        *{box-sizing:border-box;margin:0;padding:0;scroll-behavior:smooth}
        
        body{
            font-family:"Inter",-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,sans-serif;
            background:linear-gradient(135deg,var(--bg-1),var(--bg-2));
            color:var(--text);
            -webkit-font-smoothing:antialiased;
            line-height:1.6;
            min-height:100vh;
            position:relative;
            overflow-x:hidden;
        }

        body::before{
            content:"";
            position:fixed;
            top:0;
            left:0;
            width:100%;
            height:100%;
            background:
                radial-gradient(circle at 20% 20%, rgba(99, 102, 241, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 80%, rgba(167, 139, 250, 0.1) 0%, transparent 50%);
            pointer-events:none;
            z-index:0;
        }

        a{color:var(--primary-light);text-decoration:none;transition:color 0.3s ease}
        a:hover{color:var(--accent)}

        h1,h2,h3{color:var(--text);font-weight:700}
        h2{font-size:2rem;margin-bottom:1.5rem;display:flex;align-items:center;gap:0.75rem}
        h2 i{color:var(--primary-light)}

        main{
            max-width:1200px;
            margin:0 auto;
            padding:0 1.5rem 4rem;
            position:relative;
            z-index:1;
        }

        /* NAVBAR */
        header.site-header{
            position:sticky;
            top:1.25rem;
            z-index:100;
            margin:1.5rem auto 0;
            max-width:1100px;
            padding:0 1.5rem;
        }

        nav.main-nav{
            display:flex;
            justify-content:center;
            padding:0.75rem 1.5rem;
            backdrop-filter:blur(20px) saturate(180%);
            background:rgba(30, 41, 59, 0.6);
            border:1px solid var(--glass-border);
            box-shadow:var(--shadow);
            border-radius:50px;
        }

        ul.nav-links{
            display:flex;
            gap:0.5rem;
            align-items:center;
            list-style:none;
            flex-wrap:wrap;
            justify-content:center;
        }

        ul.nav-links a{
            display:inline-flex;
            gap:0.5rem;
            align-items:center;
            padding:0.625rem 1rem;
            border-radius:25px;
            color:var(--text);
            font-weight:600;
            font-size:0.875rem;
            transition:all 0.3s ease;
            position:relative;
        }

        ul.nav-links a::before{
            content:"";
            position:absolute;
            inset:0;
            border-radius:25px;
            background:linear-gradient(135deg,var(--primary),var(--accent));
            opacity:0;
            transition:opacity 0.3s ease;
        }

        ul.nav-links a:hover::before{opacity:0.15}
        ul.nav-links a:hover{transform:translateY(-2px);color:var(--primary-light)}

        /* HERO */
        section.hero{
            margin:3rem auto;
            position:relative;
            padding:4rem;
            display:flex;
            gap:3rem;
            align-items:center;
            border-radius:24px;
            background:linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(167, 139, 250, 0.1));
            backdrop-filter:blur(20px);
            border:1px solid var(--glass-border);
            box-shadow:var(--shadow);
            overflow:hidden;
        }

        section.hero::before{
            content:"";
            position:absolute;
            right:-10%;
            top:-20%;
            width:500px;
            height:500px;
            background:radial-gradient(circle, rgba(99, 102, 241, 0.3), transparent 70%);
            filter:blur(60px);
            animation:pulse 8s ease-in-out infinite;
        }

        @keyframes pulse{
            0%, 100%{transform:scale(1);opacity:0.3}
            50%{transform:scale(1.1);opacity:0.5}
        }

        section.hero .hero-left{
            display:flex;
            align-items:center;
            gap:2rem;
            z-index:2;
            flex:1;
        }

        figure.avatar{
            width:160px;
            height:160px;
            border-radius:24px;
            overflow:hidden;
            border:3px solid var(--glass-border);
            box-shadow:var(--glow);
            flex-shrink:0;
            position:relative;
        }

        figure.avatar::after{
            content:"";
            position:absolute;
            inset:0;
            background:linear-gradient(135deg, transparent, rgba(99, 102, 241, 0.2));
            opacity:0;
            transition:opacity 0.3s ease;
        }

        figure.avatar:hover::after{opacity:1}

        figure.avatar img{
            width:100%;
            height:100%;
            object-fit:cover;
            display:block;
            transition:transform 0.3s ease;
        }

        figure.avatar:hover img{transform:scale(1.05)}

        .hero-info h1{
            font-size:2.5rem;
            margin-bottom:0.5rem;
            background:linear-gradient(135deg, var(--text), var(--primary-light));
            -webkit-background-clip:text;
            -webkit-text-fill-color:transparent;
            background-clip:text;
            display:flex;
            align-items:center;
            gap:0.75rem;
        }
        
        .hero-info h1 i{
            background:linear-gradient(135deg, var(--primary), var(--accent));
            -webkit-background-clip:text;
            -webkit-text-fill-color:transparent;
            background-clip:text;
        }

        .hero-info h3{
            color:var(--text-muted);
            font-weight:500;
            font-size:1.125rem;
            margin-bottom:1.5rem;
        }

        .hero-ctas{
            display:flex;
            gap:1rem;
            align-items:center;
            flex-wrap:wrap;
        }

        .btn{
            padding:0.875rem 1.75rem;
            border-radius:12px;
            font-weight:700;
            font-size:0.9375rem;
            border:none;
            cursor:pointer;
            display:inline-flex;
            gap:0.625rem;
            align-items:center;
            transition:all 0.3s ease;
            position:relative;
            overflow:hidden;
        }

        .btn::before{
            content:"";
            position:absolute;
            inset:0;
            background:linear-gradient(135deg, transparent, rgba(255, 255, 255, 0.1));
            transform:translateX(-100%);
            transition:transform 0.3s ease;
        }

        .btn:hover::before{transform:translateX(100%)}

        .btn-primary{
            background:linear-gradient(135deg, var(--primary), var(--accent));
            color:white;
            box-shadow:0 10px 30px rgba(99, 102, 241, 0.3);
        }

        .btn-outline{
            background:transparent;
            color:var(--text);
            border:2px solid var(--glass-border);
        }

        .btn:hover{transform:translateY(-3px);box-shadow:0 15px 40px rgba(99, 102, 241, 0.4)}

        aside.hero-right{
            z-index:2;
        }

        .availability{
            background:rgba(34, 197, 94, 0.1);
            padding:1rem 1.5rem;
            border-radius:16px;
            border:1px solid rgba(34, 197, 94, 0.3);
            display:inline-block;
            backdrop-filter:blur(10px);
        }

        .availability-title{
            font-weight:700;
            font-size:1rem;
            color:#4ade80;
            display:flex;
            align-items:center;
            gap:0.5rem;
        }

        .availability-title::before{
            content:"";
            width:8px;
            height:8px;
            background:#4ade80;
            border-radius:50%;
            animation:blink 2s ease-in-out infinite;
        }

        @keyframes blink{
            0%, 100%{opacity:1}
            50%{opacity:0.3}
        }

        .availability-sub{
            font-size:0.875rem;
            color:var(--text-muted);
            margin-top:0.25rem;
        }

        ul.socials{
            margin-top:1.5rem;
            display:flex;
            gap:0.75rem;
            list-style:none;
            justify-content:flex-end;
        }

        ul.socials a{
            width:48px;
            height:48px;
            border-radius:12px;
            display:inline-flex;
            align-items:center;
            justify-content:center;
            background:rgba(99, 102, 241, 0.1);
            color:var(--primary-light);
            font-size:1.25rem;
            transition:all 0.3s ease;
            border:1px solid var(--glass-border);
        }

        ul.socials a:hover{
            transform:translateY(-4px);
            background:rgba(99, 102, 241, 0.2);
            box-shadow:var(--glow);
        }

        /* SECTIONS */
        section.block{
            margin:4rem auto 0;
            max-width:1200px;
        }

        .section-card{
            background:var(--card-bg);
            backdrop-filter:blur(20px);
            border-radius:20px;
            padding:2rem;
            box-shadow:var(--shadow);
            border:1px solid var(--glass-border);
            transition:all 0.3s ease;
            margin-top:1rem;
        }

        .section-card:hover{
            transform:translateY(-5px);
            box-shadow:0 25px 60px rgba(0, 0, 0, 0.4);
            border-color:rgba(99, 102, 241, 0.3);
        }

        p{color:var(--text-muted);margin-top:0.75rem;line-height:1.7}
        strong{color:var(--text);font-weight:600}

        ul{padding-left:1.5rem;margin-top:1rem}
        li{margin-bottom:0.75rem;color:var(--text-muted)}

        /* SKILLS */
        section.skills{text-align:center}

        section.skills img{
            width:90%;
            max-width:600px;
            border-radius:16px;
            margin:1rem 0;
            filter:drop-shadow(0 10px 30px rgba(99, 102, 241, 0.3));
        }

        /* PROJECTS */
        section.projects-list{
            display:grid;
            grid-template-columns:repeat(auto-fit, minmax(320px, 1fr));
            gap:1.5rem;
            margin-top:1rem;
        }

        article.project-card{
            padding:2rem;
            border-radius:20px;
            background:var(--card-bg);
            backdrop-filter:blur(20px);
            border:1px solid var(--glass-border);
            transition:all 0.3s ease;
            position:relative;
            overflow:hidden;
        }

        article.project-card::before{
            content:"";
            position:absolute;
            top:0;
            left:0;
            right:0;
            height:4px;
            background:linear-gradient(90deg, var(--primary), var(--accent));
            transform:scaleX(0);
            transition:transform 0.3s ease;
        }

        article.project-card:hover::before{transform:scaleX(1)}

        article.project-card:hover{
            transform:translateY(-8px);
            box-shadow:0 25px 60px rgba(99, 102, 241, 0.3);
            border-color:rgba(99, 102, 241, 0.5);
        }

        article.project-card h3{
            display:flex;
            align-items:center;
            gap:0.75rem;
            font-size:1.25rem;
            margin-bottom:0.75rem;
            color:var(--text);
        }

        article.project-card h3 i{color:var(--primary-light)}

        .meta{
            font-size:0.875rem;
            color:var(--text-muted);
            margin-bottom:1rem;
            padding:0.5rem 0;
            border-bottom:1px solid var(--glass-border);
        }

        /* EDUCATION */
        section.education-grid{
            margin-top:1rem;
            display:grid;
            grid-template-columns:repeat(auto-fit, minmax(280px, 1fr));
            gap:1.5rem;
        }

        /* FOOTER */
        footer{
            margin-top:6rem;
            padding:2rem 0;
            text-align:center;
            border-top:1px solid var(--glass-border);
            color:var(--text-muted);
            position:relative;
            z-index:1;
        }

        footer p{margin:0.5rem 0}

        /* ANIMATIONS */
        .fade-up{
            animation:fadeUp 0.8s ease both;
        }

        @keyframes fadeUp{
            from{opacity:0;transform:translateY(30px)}
            to{opacity:1;transform:translateY(0)}
        }

        .fade-up:nth-child(1){animation-delay:0.1s}
        .fade-up:nth-child(2){animation-delay:0.2s}
        .fade-up:nth-child(3){animation-delay:0.3s}
        .fade-up:nth-child(4){animation-delay:0.4s}
        .fade-up:nth-child(5){animation-delay:0.5s}
        .fade-up:nth-child(6){animation-delay:0.6s}
        .fade-up:nth-child(7){animation-delay:0.7s}

        /* RESPONSIVE */
        @media (max-width:900px){
            section.hero{
                flex-direction:column;
                padding:2.5rem 1.5rem;
                text-align:center;
            }
            
            section.hero .hero-left{
                flex-direction:column;
            }
            
            aside.hero-right{
                width:100%;
            }
            
            .availability{
                display:block;
                width:100%;
            }
            
            ul.socials{
                justify-content:center;
            }
            
            .hero-info h1{font-size:2rem}
            
            section.projects-list{
                grid-template-columns:1fr;
            }
        }

        @media (max-width:640px){
            figure.avatar{width:120px;height:120px}
            .hero-info h1{font-size:1.75rem}
            h2{font-size:1.5rem}
            main{padding:0 1rem 3rem}
            section.hero{padding:2rem 1rem}
            .section-card{padding:1.5rem}
            ul.nav-links{gap:0.25rem}
            ul.nav-links a{padding:0.5rem 0.75rem;font-size:0.8125rem}
        }
    </style>
</head>

<body>
    <header class="site-header">
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
        <section class="hero fade-up">
            <section class="hero-left">
                <figure class="avatar">
                    <img src="https://avatars.githubusercontent.com/u/0?v=4" alt="Dhruv Manohar Patel">
                </figure>
                <section class="hero-info">
                    <h1><i class="fa-solid fa-code"></i> Dhruv Manohar Patel</h1>
                    <h3>Full Stack .NET Developer • Backend Specialist • MCA Graduate</h3>
                    <section class="hero-ctas">
                        <a class="btn btn-primary" href="#projects">
                            <i class="fa-solid fa-rocket"></i> View Projects
                        </a>
                        <a class="btn btn-outline" href="mailto:dhruvpateltural@gmail.com">
                            <i class="fa-solid fa-envelope"></i> Contact
                        </a>
                    </section>
                </section>
            </section>

            <aside class="hero-right">
                <section class="availability">
                    <p class="availability-title">Open to Work</p>
                    <p class="availability-sub">Backend & .NET Roles • Remote/Hybrid</p>
                </section>

                <ul class="socials">
                    <li><a href="https://linkedin.com/in/dhruvpateltural"><i class="fab fa-linkedin"></i></a></li>
                    <li><a href="https://github.com/dhruvpateltural"><i class="fab fa-github"></i></a></li>
                    <li><a href="mailto:dhruvpateltural@gmail.com"><i class="fa-solid fa-envelope"></i></a></li>
                </ul>
            </aside>
        </section>

        <section id="about" class="block fade-up">
            <h2><i class="fa-solid fa-user"></i> About Me</h2>
            <section class="section-card">
                <p>
                    MCA graduate with <strong>full-stack development</strong> experience using
                    <strong>C#, ASP.NET, SQL Server & Entity Framework</strong>. I build
                    <strong>secure, scalable backend systems</strong>, optimize databases,
                    and work efficiently in <strong>Agile SDLC environments</strong>.
                </p>
            </section>
        </section>

        <section id="skills" class="block skills fade-up">
            <h2><i class="fa-solid fa-code"></i> Tech Stack</h2>
            <section class="section-card">
                <img src="https://skillicons.dev/icons?i=cs,dotnet,java,html,css,js,git,github,visualstudio,mysql&theme=dark"
                     alt="Technology stack icons">
                <p>C#, .NET, SQL Server, EF, ASP.NET, WinForms, HTML/CSS/JS and tooling (Git, Visual Studio)</p>
            </section>
        </section>

        <section id="internship" class="block fade-up">
            <h2><i class="fa-solid fa-briefcase"></i> Internship</h2>
            <article class="section-card">
                <h3><i class="fa-solid fa-building"></i> Software Development Intern — Aaryak Solutions</h3>
                <p class="meta"><strong>Jan 2025 – Jun 2025</strong></p>
                <ul>
                    <li>Developed 10+ backend modules using C# and ASP.NET</li>
                    <li>Improved SQL query performance by 20–30% through optimization</li>
                    <li>Implemented RBAC-based security architecture</li>
                    <li>Collaborated effectively in Agile SDLC environment</li>
                </ul>
            </article>
        </section>

        <section id="projects" class="block fade-up">
            <h2><i class="fa-solid fa-diagram-project"></i> Projects</h2>

            <section class="projects-list">
                <article class="project-card">
                    <h3><i class="fa-solid fa-utensils"></i> Restaurant Management System</h3>
                    <p class="meta"><strong>Tech:</strong> C#, ASP.NET, SQL Server, EF, HTML, CSS</p>
                    <ul>
                        <li>Automated billing, order processing and inventory management</li>
                        <li>Implemented secure role-based authentication system</li>
                        <li>Optimized backend API performance and response times</li>
                    </ul>
                </article>

                <article class="project-card">
                    <h3><i class="fa-solid fa-gears"></i> Hardware Shop Management System</h3>
                    <p class="meta"><strong>Tech:</strong> WinForms, C#, SQL Server, EF</p>
                    <ul>
                        <li>Built comprehensive sales and inventory automation</li>
                        <li>Leveraged Entity Framework ORM for reliable data handling</li>
                        <li>Created intuitive desktop interface for shop operations</li>
                    </ul>
                </article>
            </section>
        </section>

        <section id="education" class="block fade-up">
            <h2><i class="fa-solid fa-graduation-cap"></i> Education</h2>

            <section class="education-grid">
                <article class="section-card">
                    <h3>Master of Computer Applications</h3>
                    <p><strong>Finolex Academy</strong></p>
                    <p class="meta">2025 • CGPA: 8.4</p>
                </article>

                <article class="section-card">
                    <h3>Bachelor of Commerce</h3>
                    <p><strong>Gogate Jogalekar College</strong></p>
                    <p class="meta">2023 • CGPA: 8.78</p>
                </article>
            </section>
        </section>

        <section id="certifications" class="block fade-up">
            <h2><i class="fa-solid fa-certificate"></i> Certifications</h2>
            <section class="section-card">
                <ul>
                    <li><strong>Java Programming Fundamentals</strong> — SpringBoard</li>
                    <li><strong>Cyber Security & Privacy Fundamentals</strong> — NPTEL</li>
                    <li><strong>Web Development Fundamentals</strong> — IBM</li>
                </ul>
            </section>
        </section>

        <section id="achievements" class="block fade-up">
            <h2><i class="fa-solid fa-trophy"></i> Achievements</h2>

            <section class="section-card">
                <h3>Leadership & Coordination</h3>
                <ul>
                    <li><strong>Marketing Lead</strong> — Excellentia 2K25</li>
                    <li><strong>Photography & Videography Coordinator</strong> — Finolex MCA Department</li>
                </ul>
            </section>

            <section class="section-card">
                <h3>Core Strengths</h3>
                <ul>
                    <li>Problem-solving and analytical thinking</li>
                    <li>Agile collaboration and teamwork</li>
                    <li>Time management and prioritization</li>
                    <li>Adaptability and continuous learning</li>
                </ul>
            </section>
        </section>
    </main>

    <footer>
        <p>⭐ If you like my work, consider starring my repositories and connecting with me.</p>
        <p>© 2025 Dhruv Manohar Patel • Built with passion</p>
    </footer>
</body>
</html>
