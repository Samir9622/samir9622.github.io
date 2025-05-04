<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Samir9622 - GitHub Pages</title>
    <style>
        :root {
            --primary-color: #6200ee;
            --secondary-color: #03dac6;
            --dark-color: #121212;
            --light-color: #f5f5f5;
            --text-color: #333;
            --link-color: #6200ee;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
        }
        
        a {
            color: var(--link-color);
            text-decoration: none;
        }
        
        /* Header and Navigation */
        header {
            background-color: var(--primary-color);
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            color: white;
            font-size: 1.5rem;
            font-weight: bold;
            display: flex;
            align-items: center;
        }
        
        .logo::before {
            content: "</>";
            margin-right: 10px;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            color: white;
            transition: opacity 0.3s;
        }
        
        nav ul li a:hover {
            opacity: 0.8;
        }
        
        /* Hero Section */
        .hero {
            text-align: center;
            padding: 4rem 2rem;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--dark-color);
        }
        
        .hero p {
            font-size: 1.1rem;
            max-width: 800px;
            margin: 0 auto 2rem;
            color: #666;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: white;
            padding: 0.8rem 1.8rem;
            border-radius: 30px;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #5000d1;
        }
        
        /* Projects Section */
        .projects {
            background-color: #f5f5f7;
            padding: 4rem 2rem;
            text-align: center;
        }
        
        .projects h2 {
            font-size: 2rem;
            margin-bottom: 3rem;
        }
        
        .project-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 2rem;
            margin-bottom: 3rem;
        }
        
        .project-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            width: 100%;
            max-width: 350px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            text-align: left;
            transition: transform 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
        }
        
        .project-content {
            padding: 1.5rem;
        }
        
        .project-title {
            font-size: 1.2rem;
            margin-bottom: 1rem;
            color: var(--dark-color);
            display: flex;
            align-items: center;
        }
        
        .project-title .folder-icon {
            color: var(--primary-color);
            margin-right: 10px;
        }
        
        .project-links {
            display: flex;
            justify-content: space-between;
            margin-top: 1.5rem;
        }
        
        .project-link {
            display: flex;
            align-items: center;
        }
        
        .project-link i {
            margin-right: 5px;
        }
        
        /* About Section */
        .about {
            padding: 4rem 2rem;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            justify-content: center;
            gap: 3rem;
        }
        
        .about-image {
            flex: 1;
            min-width: 300px;
            max-width: 400px;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 8px;
        }
        
        .about-content {
            flex: 1;
            min-width: 300px;
            max-width: 600px;
        }
        
        .about-content h2 {
            font-size: 2rem;
            margin-bottom: 1rem;
        }
        
        .about-content h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--primary-color);
        }
        
        .about-content p {
            margin-bottom: 1.5rem;
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }
        
        .social-links a {
            font-size: 1.5rem;
            color: var(--dark-color);
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: var(--primary-color);
        }
        
        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 2rem;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .footer-top {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-bottom: 2rem;
        }
        
        .footer-brand {
            margin-bottom: 1.5rem;
        }
        
        .footer-brand h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }
        
        .footer-brand p {
            color: #aaa;
            font-size: 0.9rem;
        }
        
        .footer-nav ul {
            list-style: none;
        }
        
        .footer-nav ul li {
            margin-bottom: 0.8rem;
        }
        
        .footer-nav ul li a {
            color: #ddd;
            transition: color 0.3s;
        }
        
        .footer-nav ul li a:hover {
            color: white;
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 1.5rem;
            border-top: 1px solid #333;
            color: #aaa;
            font-size: 0.9rem;
        }
        
        /* Responsive Styles */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .about {
                flex-direction: column;
                text-align: center;
            }
            
            .about-image {
                order: 1;
            }
            
            .about-content {
                order: 2;
            }
            
            .social-links {
                justify-content: center;
            }
        }
        
        @media (max-width: 600px) {
            header {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 1rem;
            }
            
            nav ul li {
                margin-left: 0.8rem;
                margin-right: 0.8rem;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <div class="logo">Samir9622</div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="https://github.com/samir9622" target="_blank">GitHub</a></li>
            </ul>
        </nav>
    </header>
    
    <!-- Hero Section -->
    <section class="hero" id="home">
        <h1>Welcome to My GitHub Pages</h1>
        <p>Explore my projects, repositories, and coding journey. This page serves as a navigation hub for all my GitHub projects.</p>
        <a href="#projects" class="btn">Explore Projects</a>
    </section>
    
    <!-- Projects Section -->
    <section class="projects" id="projects">
        <h2>My Projects</h2>
        <div class="project-grid">
            <!-- Project Card 1 -->
            <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">
                        <span class="folder-icon"><i class="far fa-folder"></i></span>
                        Project One
                    </h3>
                    <p>Description of your first project. Explain what it does and what technologies were used.</p>
                    <div class="project-link https://samir9622.github.io/Toolhubs-1/">
                        <a href="#" class="project-link https://samir9622.github.io/Toolhubs-1/"><i class="fas fa-globe"></i> Live Demo</a>
                        <a href="#" class="project-link https://samir9622.github.io/Toolhubs-1/"><i class="fab fa-github"></i> Repository</a>
                    </div>
                </div>
            </div>
            
            <!-- Project Card 2 -->
            <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">
                        <span class="folder-icon"><i class="far fa-folder"></i></span>
                        Project Two
                    </h3>
                    <p>Description of your second project. Explain what it does and what technologies were used.</p>
                    <div class="project-link https://samir9622.github.io/Toolhubs-2/">
                        <a href="#" class="project-link https://samir9622.github.io/Toolhubs-2/"><i class="fas fa-globe"></i> Live Demo</a>
                        <a href="#" class="project-link https://samir9622.github.io/Toolhubs-2/"><i class="fab fa-github"></i> Repository</a>
                    </div>
                </div>
            </div>
            
            <!-- Project Card 3 -->
            <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">
                        <span class="folder-icon"><i class="far fa-folder"></i></span>
                        Project Three
                    </h3>
                    <p>Description of your third project. Explain what it does and what technologies were used.</p>
                    <div class="project-link https://samir9622.github.io/Tools-index.html-2/">
                        <a href="#" class="project-link https://samir9622.github.io/Tools-index.html-2/"><i class="fas fa-globe"></i> Live Demo</a>
                        <a href="#" class="project-link https://samir9622.github.io/Tools-indec.html-2/"><i class="fab fa-github"></i> Repository</a>
                    </div>
                </div>
            </div>
        </div>
        
        <a href="https://github.com/samir9622?tab=repositories" class="btn" target="_blank">
            <i class="fab fa-github"></i> View All Repositories
        </a>
    </section>
    
    <!-- About Section -->
    <section class="about" id="about">
        <div class="about-image">
            <img src="https://via.placeholder.com/400x400" alt="Profile Image">
        </div>
        <div class="about-content">
            <h2>About Me</h2>
            <h3>Samir</h3>
            <p>Welcome to my GitHub Pages website! I'm a developer passionate about creating efficient and elegant solutions to complex problems.</p>
            <p>This site serves as a portfolio and navigation hub for all my projects hosted on GitHub Pages. Feel free to explore my repositories and contact me if you have any questions or collaboration ideas.</p>
            <div class="social-links">
                <a href="https://github.com/samir9622" target="_blank"><i class="fab fa-github"></i></a>
                <a href="#" target="_blank"><i class="fab fa-linkedin"></i></a>
                <a href="mailto:your-email@example.com"><i class="fas fa-envelope"></i></a>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-top">
                <div class="footer-brand">
                    <h3>Samir9622</h3>
                    <p>Portfolio & GitHub Pages</p>
                </div>
                <div class="footer-nav">
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#projects">Projects</a></li>
                        <li><a href="#about">About</a></li>
                        <li><a href="https://github.com/samir9622" target="_blank">GitHub</a></li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <p>© 2025 Samir9622. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
