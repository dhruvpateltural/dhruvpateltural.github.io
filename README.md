
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dhruv Manohar Patel - Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --bg-light: #fafafa;
            --bg-white: #ffffff;
            --text-dark: #1a1a1a;
            --text-gray: #666666;
            --accent: #ff6b6b;
            --accent-light: #ff8787;
            --accent-dark: #ff5252;
            --border: #e0e0e0;
            --shadow: rgba(0, 0, 0, 0.08);
        }

        body {
            font-family: 'SF Pro Display', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            background: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
        }

        /* Header Navigation */
        header {
            background: var(--bg-white);
            padding: 1.5rem 5%;
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--border);
            box-shadow: 0 2px 10px var(--shadow);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--accent);
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: var(--text-dark);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            position: relative;
        }

        nav a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--accent);
            transition: width 0.3s;
        }

        nav a:hover::after {
            width: 100%;
        }

        /* Hero Section */
        .hero {
            max-width: 1200px;
            margin: 0 auto;
            padding: 5rem 2rem;
            text-align: center;
        }

        .hero h1 {
            font-size: 4rem;
            font-weight: 800;
            margin-bottom: 1rem;
            color: var(--text-dark);
            line-height: 1.2;
        }

        .gradient-text {
            background: linear-gradient(135deg, var(--accent), var(--accent-light));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: 1.5rem;
            color: var(--text-gray);
            margin-bottom: 2rem;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 1rem 2.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            display: inline-block;
            font-size: 1rem;
        }

        .btn-primary {
            background: var(--accent);
            color: white;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
        }

        .btn-primary:hover {
            background: var(--accent-dark);
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(255, 107, 107, 0.4);
        }

        .btn-outline {
            background: transparent;
            color: var(--accent);
            border: 2px solid var(--accent);
        }

        .btn-outline:hover {
            background: var(--accent);
            color: white;
        }

        /* Section Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 2rem;
        }

        .section-title {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
            text-align: center;
        }

        .section-subtitle {
            text-align: center;
            color: var(--text-gray);
            margin-bottom: 3rem;
            font-size: 1.1rem;
        }

        /* About Section */
        .about-content {
            background: var(--bg-white);
            padding: 3rem;
            border-radius: 20px;
            box-shadow: 0 10px 30px var(--shadow);
            font-size: 1.2rem;
            line-height: 1.8;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
            gap: 1.5rem;
        }

        .skill-card {
            background: var(--bg-white);
            padding: 2rem 1rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 15px var(--shadow);
            transition: all 0.3s;
            border: 2px solid transparent;
        }

        .skill-card:hover {
            transform: translateY(-10px);
            border-color: var(--accent);
            box-shadow: 0 10px 25px rgba(255, 107, 107, 0.2);
        }

        .skill-icon {
            font-size: 3rem;
            margin-bottom: 0.5rem;
        }

        .skill-name {
            font-weight: 600;
            color: var(--text-dark);
        }

        /* Experience & Projects Cards */
        .card {
            background: var(--bg-white);
            padding: 2.5rem;
            border-radius: 20px;
            box-shadow: 0 10px 30px var(--shadow);
            margin-bottom: 2rem;
            transition: all 0.3s;
            border-left: 4px solid var(--accent);
        }

        .card:hover {
            transform: translateX(10px);
            box-shadow: 0 15px 40px rgba(255, 107, 107, 0.15);
        }

        .card-header {
            display: flex;
            justify-content: space-between;
            align-items: start;
            margin-bottom: 1rem;
            flex-wrap: wrap;
            gap: 1rem;
        }

        .card-title {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--text-dark);
        }

        .card-meta {
            color: var(--text-gray);
            font-size: 0.95rem;
        }

        .card-list {
            list-style: none;
            margin-top: 1rem;
        }

        .card-list li {
            padding: 0.75rem 0;
            padding-left: 2rem;
            position: relative;
            color: var(--text-gray);
        }

        .card-list li::before {
            content: "→";
            position: absolute;
            left: 0;
            color: var(--accent);
            font-weight: bold;
        }

        /* Projects Grid */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background: var(--bg-white);
            padding: 2.5rem;
            border-radius: 20px;
            box-shadow: 0 10px 30px var(--shadow);
            transition: all 0.3s;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(255, 107, 107, 0.2);
        }

        .project-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .project-title {
            font-size: 1.6rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--text-dark);
        }

        .project-desc {
            color: var(--text-gray);
            margin-bottom: 1.5rem;
            line-height: 1.6;
        }

        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .tech-tag {
            padding: 0.4rem 1rem;
            background: linear-gradient(135deg, var(--accent), var(--accent-light));
            color: white;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 500;
        }

        /* Education Table */
        .edu-table {
            width: 100%;
            background: var(--bg-white);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 30px var(--shadow);
        }

        .edu-table th,
        .edu-table td {
            padding: 1.5rem;
            text-align: left;
        }

        .edu-table th {
            background: var(--accent);
            color: white;
            font-weight: 600;
        }

        .edu-table tr {
            border-bottom: 1px solid var(--border);
        }

        .edu-table tr:last-child {
            border-bottom: none;
        }

        .edu-table tr:hover {
            background: rgba(255, 107, 107, 0.05);
        }

        /* Certifications */
        .cert-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .cert-card {
            background: var(--bg-white);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 15px var(--shadow);
            border-top: 4px solid var(--accent);
            transition: all 0.3s;
        }

        .cert-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(255, 107, 107, 0.2);
        }

        .cert-title {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
            color: var(--text-dark);
        }

        .cert-issuer {
            color: var(--text-gray);
            font-size: 0.95rem;
        }

        /* Achievements */
        .achievements-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .achievement-card {
            background: linear-gradient(135deg, var(--accent), var(--accent-light));
            padding: 2.5rem;
            border-radius: 20px;
            color: white;
            text-align: center;
            box-shadow: 0 10px 30px rgba(255, 107, 107, 0.3);
            transition: all 0.3s;
        }

        .achievement-card:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 40px rgba(255, 107, 107, 0.4);
        }

        .achievement-icon {
            font-size: 3.5rem;
            margin-bottom: 1rem;
        }

        .achievement-title {
            font-size: 1.4rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
        }

        .achievement-desc {
            opacity: 0.9;
        }

        /* Footer CTA */
        .footer-cta {
            background: linear-gradient(135deg, var(--accent), var(--accent-light));
            color: white;
            padding: 4rem 2rem;
            text-align: center;
            border-radius: 30px;
            margin: 4rem 0;
        }

        .footer-cta h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .footer-cta p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.95;
        }

        /* Social Links */
        .social-links {
            display: flex;
            gap: 1rem;
            justify-content: center;
            margin-top: 2rem;
        }

        .social-btn {
            width: 50px;
            height: 50px;
            background: white;
            color: var(--accent);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-decoration: none;
            font-size: 1.5rem;
            transition: all 0.3s;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

        .social-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            color: var(--text-gray);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }

            .hero p {
                font-size: 1.2rem;
            }

            nav ul {
                flex-direction: column;
                gap: 1rem;
            }

            .nav-container {
                flex-direction: column;
                gap: 1rem;
            }

            .projects-grid,
            .cert-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Animations */
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

        section {
            animation: fadeInUp 0.8s ease-out;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="nav-container">
            <div class="logo">DP</div>
            <nav>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#experience">Experience</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#education">Education</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <h1>Hi, I'm <span class="gradient-text">Dhruv Manohar Patel</span></h1>
        <p>Full Stack .NET Developer | Backend Specialist | MCA Graduate</p>
        <div class="hero-buttons">
            <a href="#projects" class="btn btn-primary">View My Work</a>
            <a href="mailto:dhruvpateltural@gmail.com" class="btn btn-outline">Get In Touch</a>
        </div>
        <div class="social-links">
            <a href="https://linkedin.com/in/dhruvpateltural" class="social-btn" target="_blank">💼</a>
            <a href="https://github.com/dhruvpateltural" class="social-btn" target="_blank">🔗</a>
            <a href="mailto:dhruvpateltural@gmail.com" class="social-btn">✉️</a>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="container">
        <h2 class="section-title">About Me</h2>
        <p class="section-subtitle">Passionate developer focused on creating impactful solutions</p>
        <div class="about-content">
            MCA graduate with hands-on experience in <strong>full-stack development</strong>, specializing in the 
            <strong>C#, ASP.NET, SQL Server, and Entity Framework</strong> stack. I focus on building 
            <strong>secure, scalable applications</strong>, optimizing <strong>database performance</strong>, 
            and working in <strong>Agile SDLC environments</strong>.
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="container">
        <h2 class="section-title">Tech Stack</h2>
        <p class="section-subtitle">Technologies I work with</p>
        <div class="skills-grid">
            <div class="skill-card">
                <div class="skill-icon">💻</div>
                <div class="skill-name">C#</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">🌐</div>
                <div class="skill-name">.NET</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">🔷</div>
                <div class="skill-name">ASP.NET</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">☕</div>
                <div class="skill-name">Java</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">🗄️</div>
                <div class="skill-name">SQL Server</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">📊</div>
                <div class="skill-name">Entity Framework</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">🎨</div>
                <div class="skill-name">HTML/CSS</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">⚡</div>
                <div class="skill-name">JavaScript</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">🔧</div>
                <div class="skill-name">Git</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">🐱</div>
                <div class="skill-name">GitHub</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">🖥️</div>
                <div class="skill-name">Visual Studio</div>
            </div>
            <div class="skill-card">
                <div class="skill-icon">🐬</div>
                <div class="skill-name">MySQL</div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" class="container">
        <h2 class="section-title">Experience</h2>
        <p class="section-subtitle">My professional journey</p>
        <div class="card">
            <div class="card-header">
                <div>
                    <h3 class="card-title">🚀 Software Development Intern</h3>
                    <p class="card-meta">Aaryak Solutions</p>
                </div>
                <div class="card-meta">Jan 2025 – Jun 2025</div>
            </div>
            <ul class="card-list">
                <li>Developed <strong>10+ backend modules</strong> using C# and ASP.NET</li>
                <li>Improved <strong>SQL performance by 20–30%</strong> through query optimization</li>
                <li>Implemented <strong>RBAC security system</strong> for role-based access control</li>
                <li>Worked in full <strong>Agile SDLC lifecycle</strong> with sprint planning</li>
            </ul>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="container">
        <h2 class="section-title">Featured Projects</h2>
        <p class="section-subtitle">Some of my recent work</p>
        <div class="projects-grid">
            <div class="project-card">
                <div class="project-icon">🍽️</div>
                <h3 class="project-title">Restaurant Management System</h3>
                <p class="project-desc">
                    Complete billing, orders, and inventory management with secure RBAC authentication 
                    and optimized performance APIs.
                </p>
                <div class="tech-tags">
                    <span class="tech-tag">C#</span>
                    <span class="tech-tag">ASP.NET</span>
                    <span class="tech-tag">SQL Server</span>
                    <span class="tech-tag">Entity Framework</span>
                    <span class="tech-tag">HTML/CSS</span>
                </div>
            </div>
            <div class="project-card">
                <div class="project-icon">🔧</div>
                <h3 class="project-title">Hardware Shop Management</h3>
                <p class="project-desc">
                    Sales and inventory automation with ORM-based reliable data handling using 
                    modern desktop technologies.
                </p>
                <div class="tech-tags">
                    <span class="tech-tag">WinForms</span>
                    <span class="tech-tag">C#</span>
                    <span class="tech-tag">SQL Server</span>
                    <span class="tech-tag">Entity Framework</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education" class="container">
        <h2 class="section-title">Education</h2>
        <p class="section-subtitle">My academic background</p>
        <table class="edu-table">
            <thead>
                <tr>
                    <th>Degree</th>
                    <th>Institution</th>
                    <th>Year</th>
                    <th>CGPA</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td><strong>MCA</strong></td>
                    <td>Finolex Academy</td>
                    <td>2025</td>
                    <td><strong>8.4</strong></td>
                </tr>
                <tr>
                    <td><strong>B.Com</strong></td>
                    <td>Gogate Jogalekar College</td>
                    <td>2023</td>
                    <td><strong>8.78</strong></td>
                </tr>
            </tbody>
        </table>
    </section>

    <!-- Certifications -->
    <section class="container">
        <h2 class="section-title">Certifications</h2>
        <p class="section-subtitle">Professional credentials</p>
        <div class="cert-grid">
            <div class="cert-card">
                <h4 class="cert-title">Java Programming Fundamentals</h4>
                <p class="cert-issuer">SpringBoard</p>
            </div>
            <div class="cert-card">
                <h4 class="cert-title">Cyber Security & Privacy Fundamentals</h4>
                <p class="cert-issuer">NPTEL</p>
            </div>
            <div class="cert-card">
                <h4 class="cert-title">Web Development Fundamentals</h4>
                <p class="cert-issuer">IBM</p>
            </div>
        </div>
    </section>

    <!-- Achievements -->
    <section class="container">
        <h2 class="section-title">Achievements & Leadership</h2>
        <p class="section-subtitle">Making an impact beyond code</p>
        <div class="achievements-grid">
            <div class="achievement-card">
                <div class="achievement-icon">🏅</div>
                <h3 class="achievement-title">Marketing Lead</h3>
                <p class="achievement-desc">Excellentia 2K25</p>
            </div>
            <div class="achievement-card">
                <div class="achievement-icon">📸</div>
                <h3 class="achievement-title">Photography & Videography</h3>
                <p class="achievement-desc">Finolex MCA Department</p>
            </div>
            <div class="achievement-card">
                <div class="achievement-icon">🧩</div>
                <h3 class="achievement-title">Problem Solver</h3>
                <p class="achievement-desc">Analytical Thinking Expert</p>
            </div>
            <div class="achievement-card">
                <div class="achievement-icon">🤝</div>
                <h3 class="achievement-title">Team Player</h3>
                <p class="achievement-desc">Agile Collaboration</p>
            </div>
        </div>
    </section>

    <!-- Footer CTA -->
    <section id="contact" class="container">
        <div class="footer-cta">
            <h2>🚀 Career Objective</h2>
            <p>
                To work as a <strong>Full Stack .NET Developer</strong> in building secure, scalable, 
                and high-performance enterprise applications.
            </p>
            <a href="mailto:dhruvpateltural@gmail.com" class="btn" style="background: white; color: var(--accent);">Let's Work Together</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>© 2025 Dhruv Manohar Patel. Built with passion and .NET</p>
    </footer>

    <script>
        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });

        // Scroll animation
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('section').forEach(section => {
            section.style.opacity = '0';
            section.style.transform = 'translateY(20px)';
            section.style.transition = 'all 0.6s ease-out';
            observer.observe(section);
        });
    </script>
</body>
</html>
