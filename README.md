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
    <style>
    :root {
    --bg-primary: #ffffff;
    --bg-secondary: #fafafa;
    --bg-tertiary: #f8f9fa;
    --text-primary: #000000;
    --text-secondary: #4a5568;
    --text-muted: #718096;
    --accent: #3182ce;
    --accent-hover: #2c5aa0;
    --accent-light: #ebf4ff;
    --border: #e2e8f0;
    --border-light: #f1f5f9;
    --shadow-subtle: rgba(0, 0, 0, 0.03);
    --shadow-soft: rgba(0, 0, 0, 0.06);
    --shadow-medium: rgba(0, 0, 0, 0.1);
    --shadow-strong: rgba(0, 0, 0, 0.15);
    --transition-smooth: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    --transition-quick: all 0.2s cubic-bezier(0.4, 0, 0.2, 1);
    --transition-slow: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
    --radius-xs: 2px;
    --radius-sm: 4px;
    --radius-md: 6px;
    --radius-lg: 8px;
    --radius-xl: 12px;
    --radius-2xl: 16px;
    --space-1: 0.25rem;
    --space-2: 0.5rem;
    --space-3: 0.75rem;
    --space-4: 1rem;
    --space-5: 1.25rem;
    --space-6: 1.5rem;
    --space-8: 2rem;
    --space-10: 2.5rem;
    --space-12: 3rem;
    --space-16: 4rem;
    --space-20: 5rem;
}


/* Dark theme with enhanced contrast */

[data-theme="dark"] {
    --bg-primary: #000000;
    --bg-secondary: #0d1117;
    --bg-tertiary: #161b22;
    --text-primary: #f0f6fc;
    --text-secondary: #c9d1d9;
    --text-muted: #8b949e;
    --accent: #58a6ff;
    --accent-hover: #79c0ff;
    --accent-light: rgba(88, 166, 255, 0.1);
    --border: #30363d;
    --border-light: #21262d;
    --shadow-subtle: rgba(255, 255, 255, 0.03);
    --shadow-soft: rgba(255, 255, 255, 0.06);
    --shadow-medium: rgba(255, 255, 255, 0.1);
    --shadow-strong: rgba(255, 255, 255, 0.15);
}


/* Reset and Base with Font Optimization */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    font-display: swap;
}

body {
    font-family: -apple-system, BlinkMacSystemFont, 'SF Pro Display', 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    font-size: clamp(15px, 2.5vw, 16px);
    font-weight: 400;
    line-height: 1.6;
    letter-spacing: -0.01em;
    color: var(--text-primary);
    background: var(--bg-primary);
    transition: var(--transition-smooth);
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-rendering: optimizeLegibility;
}


/* Enhanced Header with Perfect Alignment */

header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
    padding: var(--space-6) var(--space-8);
    background: rgba(255, 255, 255, 0.8);
    backdrop-filter: blur(20px);
    -webkit-backdrop-filter: blur(20px);
    border-bottom: 1px solid var(--border);
    transition: var(--transition-smooth);
}

[data-theme="dark"] header {
    background: rgba(13, 17, 23, 0.8);
}

nav {
    max-width: 1400px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: var(--space-8);
}

.nav-item {
    display: flex;
    align-items: center;
    gap: var(--space-2);
    position: relative;
}

.nav-item span {
    color: var(--text-muted);
    font-size: 12px;
    font-weight: 500;
    transition: var(--transition-quick);
}

.nav-item a {
    color: var(--text-primary);
    text-decoration: none;
    font-weight: 500;
    font-size: 14px;
    opacity: 0.7;
    transition: var(--transition-quick);
    padding: var(--space-2) var(--space-3);
    border-radius: var(--radius-md);
    position: relative;
}

.nav-item:hover span {
    color: var(--accent);
    transform: scale(1.2);
}

.nav-item:hover a {
    opacity: 1;
    color: var(--accent);
    background: var(--accent-light);
}


/* Perfect Theme Toggle */

.theme-toggle {
    display: flex;
    align-items: center;
}

#theme-btn {
    background: transparent;
    border: 1px solid var(--border);
    color: var(--text-primary);
    padding: var(--space-2) var(--space-4);
    border-radius: var(--radius-2xl);
    cursor: pointer;
    font-size: 13px;
    font-weight: 500;
    transition: var(--transition-smooth);
    position: relative;
    overflow: hidden;
}

#theme-btn:hover {
    background: var(--accent);
    color: #ffffff;
    border-color: var(--accent);
    transform: translateY(-2px);
    box-shadow: 0 4px 12px var(--shadow-medium);
}

#theme-btn:active {
    transform: translateY(0);
}


/* Enhanced Hero Section with Perfect Typography */

.hero-section {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: var(--space-16) var(--space-6);
    position: relative;
    background: var(--bg-primary);
    overflow: hidden;
}

.hero-section::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(circle at 30% 40%, var(--accent-light) 0%, transparent 50%);
    pointer-events: none;
    opacity: 0.5;
}

.hero-content {
    text-align: center;
    max-width: 900px;
    z-index: 2;
    position: relative;
}

.hero-content h1 {
    font-size: clamp(2.5rem, 7vw, 5rem);
    font-weight: 700;
    line-height: 0.9;
    margin-bottom: var(--space-4);
    letter-spacing: -0.03em;
    color: var(--text-primary);
    opacity: 0;
    transform: translateY(30px);
    animation: heroFadeIn 1.2s cubic-bezier(0.4, 0, 0.2, 1) forwards;
}

.hero-content p {
    font-size: clamp(1rem, 2vw, 1.25rem);
    font-weight: 400;
    color: var(--text-secondary);
    margin-bottom: var(--space-8);
    letter-spacing: -0.005em;
    opacity: 0;
    transform: translateY(20px);
    animation: heroFadeIn 1.2s cubic-bezier(0.4, 0, 0.2, 1) 0.2s forwards;
}

@keyframes heroFadeIn {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}


/* Enhanced Content Sections */

.content-section {
    padding: var(--space-20) var(--space-6);
    max-width: 1200px;
    margin: 0 auto;
    position: relative;
    opacity: 0;
    transform: translateY(40px);
    transition: var(--transition-slow);
}

.content-section.visible {
    opacity: 1;
    transform: translateY(0);
}

.section-content {
    max-width: 900px;
    margin: 0 auto;
}

.section-content h2 {
    font-size: clamp(2rem, 4vw, 3rem);
    font-weight: 600;
    margin-bottom: var(--space-8);
    line-height: 1.1;
    letter-spacing: -0.02em;
    color: var(--text-primary);
    position: relative;
}

.section-content h2::after {
    content: '';
    position: absolute;
    bottom: -var(--space-3);
    left: 0;
    width: 60px;
    height: 3px;
    background: var(--accent);
    border-radius: var(--radius-xs);
}

.section-content p {
    font-size: 1.1rem;
    line-height: 1.7;
    color: var(--text-secondary);
    margin-bottom: var(--space-6);
}


/* Enhanced Download Button */

.download-btn {
    display: inline-flex;
    align-items: center;
    gap: var(--space-2);
    padding: var(--space-3) var(--space-6);
    background: var(--accent);
    color: #ffffff;
    text-decoration: none;
    font-weight: 500;
    font-size: 15px;
    border-radius: var(--radius-lg);
    transition: var(--transition-smooth);
    border: 1px solid var(--accent);
    position: relative;
    overflow: hidden;
}

.download-btn:hover {
    background: var(--accent-hover);
    border-color: var(--accent-hover);
    transform: translateY(-2px);
    box-shadow: 0 8px 20px var(--shadow-medium);
}


/* Enhanced Projects Grid */

.projects-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: var(--space-8);
    margin-top: var(--space-10);
}

.project-item {
    background: var(--bg-primary);
    border: 1px solid var(--border);
    border-radius: var(--radius-xl);
    padding: var(--space-8);
    transition: var(--transition-smooth);
    position: relative;
    overflow: hidden;
}

.project-item::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 3px;
    background: var(--accent);
    transform: scaleX(0);
    transition: var(--transition-smooth);
}

.project-item:hover {
    border-color: var(--accent);
    box-shadow: 0 20px 40px var(--shadow-soft);
    transform: translateY(-8px);
}

.project-item:hover::before {
    transform: scaleX(1);
}

.project-item h3 {
    font-size: 1.4rem;
    font-weight: 600;
    margin-bottom: var(--space-3);
    color: var(--text-primary);
    line-height: 1.3;
}

.project-item p {
    font-size: 1rem;
    line-height: 1.6;
    color: var(--text-secondary);
    margin-bottom: var(--space-5);
}

.project-link {
    display: inline-flex;
    align-items: center;
    color: var(--accent);
    text-decoration: none;
    font-weight: 500;
    font-size: 14px;
    transition: var(--transition-quick);
    position: relative;
}

.project-link::after {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--accent);
    transition: var(--transition-smooth);
}

.project-link:hover::after {
    width: 100%;
}


/* Enhanced Skills Grid */

.skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: var(--space-8);
    margin-top: var(--space-10);
}

.skill-category h3 {
    font-size: 1.1rem;
    font-weight: 600;
    margin-bottom: var(--space-4);
    color: var(--text-primary);
}

.skill-category ul {
    list-style: none;
}

.skill-category li {
    color: var(--text-secondary);
    font-size: 0.95rem;
    margin-bottom: var(--space-2);
    padding: var(--space-2) 0 var(--space-2) var(--space-2);
    border-left: 2px solid var(--border);
    transition: var(--transition-quick);
}

.skill-category li:hover {
    color: var(--text-primary);
    border-left-color: var(--accent);
    padding-left: var(--space-4);
}


/* Enhanced Contact Section */

.contact-link {
    display: inline-flex;
    align-items: center;
    gap: var(--space-2);
    color: var(--accent);
    text-decoration: none;
    font-weight: 500;
    font-size: 15px;
    padding: var(--space-3) var(--space-5);
    border: 1px solid var(--accent);
    border-radius: var(--radius-lg);
    transition: var(--transition-smooth);
    background: transparent;
}

.contact-link:hover {
    background: var(--accent);
    color: #ffffff;
    transform: translateY(-2px);
    box-shadow: 0 6px 16px var(--shadow-medium);
}


/* Enhanced Footer */

footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: var(--space-8) var(--space-6);
    background: var(--bg-secondary);
    border-top: 1px solid var(--border);
    margin-top: var(--space-20);
}

footer p {
    color: var(--text-muted);
    font-size: 14px;
}

footer a {
    color: var(--text-secondary);
    text-decoration: none;
    font-weight: 500;
    transition: var(--transition-quick);
}

footer a:hover {
    color: var(--accent);
}


/* Wave/Visual Guards */

.grid-container,
.grid-layer,
.grid-line,
.grid-dot,
.floating-element,
.geometric-hero {
    display: none !important;
}


/* Enhanced Animations */

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


/* Responsive Design Perfection */

@media (max-width: 768px) {
    header {
        padding: var(--space-4) var(--space-4);
    }
    nav {
        flex-direction: column;
        gap: var(--space-4);
    }
    .nav-item {
        flex-direction: column;
        gap: var(--space-1);
    }
    .hero-section {
        padding: var(--space-12) var(--space-4);
        min-height: 80vh;
    }
    .content-section {
        padding: var(--space-12) var(--space-4);
    }
    .projects-grid,
    .skills-grid {
        grid-template-columns: 1fr;
        gap: var(--space-6);
    }
    footer {
        flex-direction: column;
        gap: var(--space-3);
        text-align: center;
    }
}

@media (max-width: 480px) {
    .hero-content h1 {
        font-size: clamp(2rem, 10vw, 3rem);
    }
    .hero-content p {
        font-size: clamp(0.9rem, 4vw, 1rem);
    }
    .section-content h2 {
        font-size: clamp(1.5rem, 6vw, 2rem);
    }
    .section-content p {
        font-size: 1rem;
    }
    .project-item,
    .skill-category {
        padding: var(--space-6);
    }
}


/* Performance and Accessibility */

@media (prefers-reduced-motion: reduce) {
    *,
    *::before,
    *::after {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
    }
}


/* Focus States for Accessibility */

a:focus,
button:focus,
input:focus {
    outline: 2px solid var(--accent);
    outline-offset: 2px;
    border-radius: var(--radius-sm);
}


/* Print Styles */

@media print {
    header,
    footer {
        display: none;
    }
    .hero-section {
        min-height: auto;
        padding: var(--space-4);
    }
    .content-section {
        padding: var(--space-4);
    }
}</style>
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

