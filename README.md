### Welcome on board to the best dev site
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>David Costin | Portfolio</title>
    <link rel="stylesheet" href="codigo.css" />
    <link rel="stylesheet" href="geometric-grid.css" />
    <meta name="description" content="Software Developer portfolio showcasing projects and skills">
    <meta name="keywords" content="software developer, portfolio, web development, programming">
    <meta name="author" content="David Costin">
</head>

<body>
    <header>
        <nav>
            <div class="nav-item">
                <span>●</span>
                <a href="#top">Home</a>
            </div>
            <div class="nav-item">
                <span>●</span>
                <a href="#about">About</a>
            </div>
            <div class="nav-item">
                <span>●</span>
                <a href="#projects">Projects</a>
            </div>
            <div class="nav-item">
                <span>●</span>
                <a href="#skills">Skills</a>
            </div>
            <div class="nav-item">
                <span>●</span>
                <a href="#contact">Contact</a>
            </div>
            <div class="theme-toggle">
                <button id="theme-btn">Light</button>
            </div>
        </nav>
    </header>
    <main>
        <section id="top" class="hero-section">
            <div class="hero-content">
                <h1>David Costin</h1>
                <p>Software Developer</p>
            </div>
        </section>
        <section id="about" class="content-section">
            <div class="section-content">
                <h2>About</h2>
                <p>
                    Second-year student of Multiplatform Application Development, with great interest in programming, cybersecurity, and software development. I am characterized by a high learning capacity, a methodical approach to problem-solving, and a collaborative attitude
                    in teamwork. My goal is to join a technology company where I can apply the knowledge acquired during my training, contribute value from the start, and continue to develop professionally in a demanding, dynamic, and continuous improvement-oriented
                    environment.
                </p>
                <a href="David-Robert-Costin-Curriculum.pdf" class="download-btn" download>
                Download Resume
            </a>
            </div>
        </section>
        <section id="projects" class="content-section">
            <div class="section-content">
                <h2>Projects</h2>
                <div class="projects-grid">
                    <div class="project-item">
                        <h3>E-commerce Platform</h3>
                        <p>Full-stack web application with React, Node.js, and MongoDB. User authentication, payment integration, and admin dashboard.</p>
                        <a href="#" class="project-link">View Project</a>
                    </div>
                    <div class="project-item">
                        <h3>Mobile Weather App</h3>
                        <p>React Native application with real-time weather data, location services, and beautiful UI components.</p>
                        <a href="#" class="project-link">View Project</a>
                    </div>
                    <div class="project-item">
                        <h3>Data Visualization Tool</h3>
                        <p>Interactive dashboard using D3.js and Python for analyzing complex datasets with real-time updates.</p>
                        <a href="#" class="project-link">View Project</a>
                    </div>
                    <div class="project-item">
                        <h3>Task Management System</h3>
                        <p>Collaborative project management tool with real-time updates, file sharing, and team communication features.</p>
                        <a href="#" class="project-link">View Project</a>
                    </div>
                </div>
            </div>
        </section>
        <section id="skills" class="content-section">
            <div class="section-content">
                <h2>Skills</h2>
                <div class="skills-grid">
                    <div class="skill-category">
                        <h3>Frontend</h3>
                        <ul>
                            <li>HTML/CSS</li>
                            <li>JavaScript</li>
                            <li>React</li>
                            <li>TypeScript</li>
                        </ul>
                    </div>
                    <div class="skill-category">
                        <h3>Backend</h3>
                        <ul>
                            <li>Python</li>
                            <li>Node.js</li>
                            <li>Java</li>
                            <li>PostgreSQL</li>
                        </ul>
                    </div>
                    <div class="skill-category">
                        <h3>Mobile</h3>
                        <ul>
                            <li>React Native</li>
                            <li>Kotlin</li>
                            <li>Flutter</li>
                        </ul>
                    </div>
                    <div class="skill-category">
                        <h3>Tools</h3>
                        <ul>
                            <li>Git</li>
                            <li>Docker</li>
                            <li>AWS</li>
                            <li>CI/CD</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>
        <section id="contact" class="content-section">
            <div class="section-content">
                <h2>Contact</h2>
                <p>Always interested in new opportunities and collaborations. Feel free to reach out!</p>
                <div style="display: flex; gap: 2rem; margin-top: 2rem; flex-wrap: wrap;">
                    <a href="mailto:davidcstin25@gmail.com" class="contact-link">Email</a>
                    <a href="https://github.com" target="_blank" class="contact-link">GitHub</a>
                    <a href="https://linkedin.com" target="_blank" class="contact-link">LinkedIn</a>
                </div>
            </div>
        </section>
        <footer>
            <p>© 2026 David Costin</p>
            <a href="#top">Back to Top</a>
        </footer>
        <script src="animations.js"></script>
        <script>
            // Enhanced animations and interactions
            document.addEventListener('DOMContentLoaded', () => {
                // Hero fade-in animation
                const heroTitle = document.querySelector('.hero-content h1');
                const heroSubtitle = document.querySelector('.hero-content p');
                if (heroTitle) {
                    heroTitle.style.opacity = '0';
                    heroTitle.style.transform = 'translateY(30px)';
                    setTimeout(() => {
                        heroTitle.style.transition = 'all 1.2s cubic-bezier(0.4, 0, 0.2, 1)';
                        heroTitle.style.opacity = '1';
                        heroTitle.style.transform = 'translateY(0)';
                    }, 300);
                }
                if (heroSubtitle) {
                    heroSubtitle.style.opacity = '0';
                    heroSubtitle.style.transform = 'translateY(20px)';
                    setTimeout(() => {
                        heroSubtitle.style.transition = 'all 1.2s cubic-bezier(0.4, 0, 0.2, 1)';
                        heroSubtitle.style.opacity = '1';
                        heroSubtitle.style.transform = 'translateY(0)';
                    }, 500);
                }
                // Intersection Observer for sections
                const observer = new IntersectionObserver((entries) => {
                    entries.forEach(entry => {
                        if (entry.isIntersecting) {
                            entry.target.classList.add('visible');
                        }
                    });
                }, {
                    threshold: 0.1
                });
                document.querySelectorAll('.content-section').forEach(section => {
                    section.style.opacity = '0';
                    section.style.transform = 'translateY(40px)';
                    section.style.transition = 'all 0.6s cubic-bezier(0.4, 0, 0.2, 1)';
                    observer.observe(section);
                });
            });
        </script>

</body>

</html>
