
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dhruv Manohar Patel - Full Stack .NET Developer</title>
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
            flex-wrap: wrap;
        }

        nav a {
            color: var(--light);
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
            background: linear-gradient(90deg, var(--primary), var(--secondary));
            transition: width 0.3s;
        }

        nav a:hover::after {
            width: 100%;
        }

        /* Hero Section */
        .hero {
            position: relative;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 2rem;
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
            nav ul { gap: 1rem; }
        }
    </style>
</head>
<body>
    <!-- Animated Background -->
    <div class="bg-animation" id="bgAnimation"></div>

    <!-- Navigation -->
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

    <!-- Hero Section -->
    <div class="hero">
        <div class="hero-content">
            <h1>Dhruv Manohar Patel</h1>
            <p class="subtitle">Full Stack .NET Developer | Backend Specialist | MCA Graduate</p>
            <div class="social-links">
                <a href="https://linkedin.com/in/dhruvpateltural" class="social-btn linkedin" target="_blank">LinkedIn</a>
                <a href="https://github.com/dhruvpateltural" class="social-btn github" target="_blank">GitHub</a>
                <a href="mailto:dhruvpateltural@gmail.com" class="social-btn email">Email Me</a>
            </div>
        </div>
    </div>

    <!-- About Section -->
    <section id="about">
        <h2 class="section-title">About Me</h2>
        <div class="card">
            <p style="font-size: 1.2rem; line-height: 1.8;">
                MCA graduate with hands-on experience in <strong>full-stack development</strong>, specializing in the 
                <strong>C#, ASP.NET, SQL Server, and Entity Framework</strong> stack. I focus on building 
                <strong>secure, scalable applications</strong>, optimizing <strong>database performance</strong>, 
                and working in <strong>Agile SDLC environments</strong>.
            </p>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <h2 class="section-title">Tech Stack</h2>
        <div class="skills-grid">
            <div class="skill-item">
                <div class="skill-icon">💻</div>
                <div>C#</div>
            </div>
            <div class="skill-item">
                <div class="skill-icon">🌐</div>
                <div>.NET</div>
            </div>
            <div class="skill-item">
                <div class="skill-icon">☕</div>
                <div>Java</div>
            </div>
            <div class="skill-item">
                <div class="skill-icon">🗄️</div>
                <div>SQL Server</div>
            </div>
            <div class="skill-item">
                <div class="skill-icon">📊</div>
                <div>Entity Framework</div>
            </div>
            <div class="skill-item">
                <div class="skill-icon">🎨</div>
                <div>HTML/CSS</div>
            </div>
            <div class="skill-item">
                <div class="skill-icon">⚡</div>
                <div>JavaScript</div>
            </div>
            <div class="skill-item">
                <div class="skill-icon">🔧</div>
                <div>Git</div>
            </div>
        </div>
    </section>

    <!-- Internship Section -->
    <section id="internship">
        <h2 class="section-title">Experience</h2>
        <div class="card">
            <h3 style="color: var(--accent); font-size: 1.8rem;">🚀 Software Development Intern</h3>
            <p style="color: #888; margin: 0.5rem 0;"><strong>Aaryak Solutions</strong> | Jan 2025 – Jun 2025</p>
            <ul style="margin-top: 1rem; line-height: 2;">
                <li>✅ Developed <strong>10+ backend modules</strong></li>
                <li>✅ Improved <strong>SQL performance by 20–30%</strong></li>
                <li>✅ Implemented <strong>RBAC security system</strong></li>
                <li>✅ Worked in full <strong>Agile SDLC lifecycle</strong></li>
            </ul>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects">
        <h2 class="section-title">Projects</h2>
        <div class="projects-grid">
            <div class="project-card">
                <h3>🍽️ Restaurant Management System</h3>
                <p>Complete billing, orders, and inventory management with secure RBAC authentication and optimized performance APIs.</p>
                <div class="tech-stack">
                    <span class="tech-tag">C#</span>
                    <span class="tech-tag">ASP.NET</span>
                    <span class="tech-tag">SQL Server</span>
                    <span class="tech-tag">Entity Framework</span>
                    <span class="tech-tag">HTML/CSS</span>
                </div>
            </div>
            <div class="project-card">
                <h3>🔧 Hardware Shop Management System</h3>
                <p>Sales and inventory automation with ORM-based reliable data handling using modern desktop technologies.</p>
                <div class="tech-stack">
                    <span class="tech-tag">WinForms</span>
                    <span class="tech-tag">C#</span>
                    <span class="tech-tag">SQL Server</span>
                    <span class="tech-tag">Entity Framework</span>
                </div>
            </div>
        </div>
    </section>

    <!-- Education Section -->
    <section id="education">
        <h2 class="section-title">Education</h2>
        <div class="card">
            <table>
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
                        <td><strong style="color: var(--accent);">8.4</strong></td>
                    </tr>
                    <tr>
                        <td><strong>B.Com</strong></td>
                        <td>Gogate Jogalekar College</td>
                        <td>2023</td>
                        <td><strong style="color: var(--accent);">8.78</strong></td>
                    </tr>
                </tbody>
            </table>
        </div>

        <h2 class="section-title" style="margin-top: 4rem;">Certifications</h2>
        <div class="timeline">
            <div class="timeline-item">
                <div class="card">
                    <h4>Java Programming Fundamentals</h4>
                    <p style="color: #888;">SpringBoard</p>
                </div>
            </div>
            <div class="timeline-item">
                <div class="card">
                    <h4>Cyber Security & Privacy Fundamentals</h4>
                    <p style="color: #888;">NPTEL</p>
                </div>
            </div>
            <div class="timeline-item">
                <div class="card">
                    <h4>Web Development Fundamentals</h4>
                    <p style="color: #888;">IBM</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Achievements Section -->
    <section id="achievements">
        <h2 class="section-title">Achievements & Leadership</h2>
        <div class="achievements-grid">
            <div class="achievement-badge">
                <div class="badge-icon">🏅</div>
                <h4>Marketing Lead</h4>
                <p>Excellentia 2K25</p>
            </div>
            <div class="achievement-badge">
                <div class="badge-icon">📸</div>
                <h4>Photography & Videography</h4>
                <p>Finolex MCA Department</p>
            </div>
            <div class="achievement-badge">
                <div class="badge-icon">🧩</div>
                <h4>Problem Solving</h4>
                <p>Analytical Thinking</p>
            </div>
            <div class="achievement-badge">
                <div class="badge-icon">🤝</div>
                <h4>Agile Collaboration</h4>
                <p>Team Player</p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <h3 style="margin-bottom: 1rem;">🚀 Career Objective</h3>
        <p style="font-size: 1.1rem; max-width: 800px; margin: 0 auto; line-height: 1.8;">
            To work as a <strong>Full Stack .NET Developer</strong> in building <strong>secure, scalable, 
            and high-performance enterprise applications</strong>.
        </p>
        <p style="margin-top: 2rem; color: #888;">
            ⭐ If you like my work, consider starring my repositories and connecting with me!
        </p>
    </footer>

    <script>
        // Create animated background particles
        const bgAnimation = document.getElementById('bgAnimation');
        for (let i = 0; i < 50; i++) {
            const span = document.createElement('span');
            span.style.left = Math.random() * 100 + '%';
            span.style.animationDelay = Math.random() * 15 + 's';
            span.style.animationDuration = (Math.random() * 10 + 10) + 's';
            bgAnimation.appendChild(span);
        }

        // Smooth scroll for navigation
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                target.scrollIntoView({ behavior: 'smooth', block: 'start' });
            });
        });

        // Intersection Observer for fade-in animations
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animation = 'fadeInUp 0.8s ease-out';
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.card, .project-card, .achievement-badge').forEach(el => {
            observer.observe(el);
        });
    </script>
</body>
</html>
