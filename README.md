علي مهدي 77, [6/20/2025 9:53 PM]
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ali Abdulal Mahdi - Portfolio</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #3498db;
            --secondary: #2ecc71;
            --dark: #2c3e50;
            --light: #ecf0f1;
            --accent: #e74c3c;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: var(--dark);
            color: var(--light);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        header {
            text-align: center;
            padding: 3rem 0;
            animation: fadeIn 1.5s ease-in-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            background: linear-gradient(45deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            display: inline-block;
        }
        
        .tagline {
            font-size: 1.2rem;
            opacity: 0.9;
            margin-bottom: 2rem;
        }
        
        .contact-info {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-bottom: 3rem;
            flex-wrap: wrap;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            transition: transform 0.3s ease;
        }
        
        .contact-item:hover {
            transform: translateY(-5px);
            color: var(--secondary);
        }
        
        .section {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 2rem;
            margin-bottom: 2rem;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            animation: slideUp 1s ease-in-out;
            animation-fill-mode: both;
        }
        
        @keyframes slideUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .section:nth-child(2) { animation-delay: 0.2s; }
        .section:nth-child(3) { animation-delay: 0.4s; }
        .section:nth-child(4) { animation-delay: 0.6s; }
        .section:nth-child(5) { animation-delay: 0.8s; }
        
        h2 {
            font-size: 2rem;
            margin-bottom: 1.5rem;
            color: var(--primary);
            position: relative;
            display: inline-block;
        }
        
        h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 50px;
            height: 3px;
            background: var(--secondary);
            border-radius: 3px;
        }
        
        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
        }
        
        .skill {
            background: rgba(255, 255, 255, 0.2);
            padding: 0.8rem 1.2rem;
            border-radius: 50px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            transition: all 0.3s ease;
        }
        
        .skill:hover {
            background: var(--primary);
            transform: scale(1.05);
        }
        
        .projects-grid {
            display: grid;

علي مهدي 77, [6/20/2025 9:53 PM]
grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 1.5rem;
        }
        
        .project-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 1.5rem;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
            border-color: var(--primary);
        }
        
        .project-title {
            font-size: 1.3rem;
            margin-bottom: 0.5rem;
            color: var(--secondary);
        }
        
        .project-links {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }
        
        .btn {
            padding: 0.5rem 1rem;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
        }
        
        .btn-primary {
            background: var(--primary);
            color: white;
        }
        
        .btn-primary:hover {
            background: #2980b9;
        }
        
        .btn-outline {
            border: 1px solid var(--primary);
            color: var(--primary);
        }
        
        .btn-outline:hover {
            background: var(--primary);
            color: white;
        }
        
        footer {
            text-align: center;
            padding: 2rem 0;
            margin-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            animation: fadeIn 1s ease-in-out;
        }
        
        .signature {
            font-family: 'Dancing Script', cursive;
            font-size: 2rem;
            background: linear-gradient(45deg, var(--primary), var(--accent));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            display: inline-block;
            margin-top: 1rem;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 1rem;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .projects-grid {
                grid-template-columns: 1fr;
            }
        }
        
        /* Animation for skills */
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        .pulse {
            animation: pulse 2s infinite;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Ali Abdulal Mahdi</h1>
            <p class="tagline">Computer Science Student | Full Stack Developer</p>
            <div class="contact-info">
                <div class="contact-item">
                    <i class="fas fa-envelope"></i>
                    <a href="mailto:ali.mahdi.67.99@gmail.com" style="color: inherit; text-decoration: none;">ali.mahdi.67.99@gmail.com</a>
                </div>
                <div class="contact-item">
                    <i class="fas fa-university"></i>
                    <a href="mailto:ali.abdulalmahdi.sci25@st.nahrainuniv.edu.iq" style="color: inherit; text-decoration: none;">University Email</a>
                </div>
                <div class="contact-item">
                    <i class="fab fa-github"></i>
                    <a href="https://github.com/AliAbdulalMahdi" target="_blank" style="color: inherit; text-decoration: none;">GitHub</a>
                </div>
            </div>
        </header>
        
        <section class="section">
            <h2>Technical Skills</h2>
            <div class="skills-container">
                <div class="skill pulse">
                    <i class="fab fa-java"></i>
                    <span>Java (Expert)</span>
                </div>

علي مهدي 77, [6/20/2025 9:53 PM]
<div class="skill pulse">
                    <i class="fas fa-code"></i>
                    <span>C# (Intermediate)</span>
                </div>
                <div class="skill pulse">
                    <i class="fab fa-html5"></i>
                    <span>HTML5 (Advanced)</span>
                </div>
                <div class="skill pulse">
                    <i class="fab fa-css3-alt"></i>
                    <span>CSS3 (Advanced)</span>
                </div>
                <div class="skill pulse">
                    <i class="fab fa-github"></i>
                    <span>GitHub (Proficient)</span>
                </div>
            </div>
        </section>
        
        <section class="section">
            <h2>Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <h3 class="project-title">Task Management System</h3>
                    <p>A console-based task management application using Java OOP principles.</p>
                    <div class="project-links">
                        <a href="#" class="btn btn-primary">
                            <i class="fab fa-github"></i> View Code
                        </a>
                    </div>
                </div>
                <div class="project-card">
                    <h3 class="project-title">Personal Portfolio</h3>
                    <p>A responsive portfolio website built with HTML and CSS.</p>
                    <div class="project-links">
                        <a href="#" class="btn btn-primary">
                            <i class="fab fa-github"></i> View Code
                        </a>
                        <a href="#" class="btn btn-outline">
                            <i class="fas fa-external-link-alt"></i> Live Demo
                        </a>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="section">
            <h2>Education</h2>
            <div style="margin-bottom: 1rem;">
                <h3 style="color: var(--secondary);">Al-Nahrain University</h3>
                <p>Bachelor of Science in Computer Science (Expected 2025)</p>
            </div>
        </section>
        
        <section class="section">
            <h2>Get Started with My Projects</h2>
            <pre style="background: rgba(0, 0, 0, 0.3); padding: 1rem; border-radius: 5px; overflow-x: auto;">
                <code>
# Clone the project
git clone https://github.com/AliAbdulalMahdi/ProjectName.git

# Navigate to project directory
cd ProjectName

# Run the application (Java example)
javac Main.java
java Main
                </code>
            </pre>
        </section>
        
        <footer>
            <p>© 2024 Ali Abdulal Mahdi. All projects are licensed under MIT License.</p>
            <p style="margin-top: 0.5rem;">"Clean code is an expression of professionalism"</p>
            <div class="signature">Ali Abdulal Mahdi</div>
            <p style="margin-top: 2rem;">Last updated: July 15, 2024</p>
        </footer>
    </div>
</body>
</html>
