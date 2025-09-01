<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Portfolio of Sachindra Shekhar Pandey, AI/ML Engineer and Space Tech Pioneer. Explore projects in weather nowcasting, crowd management, and more.">
    <meta name="keywords" content="AI Engineer, ML Developer, Space Technology, Weather Prediction, Computer Vision">
    <meta property="og:title" content="Sachindra Shekhar Pandey - AI/ML Engineer">
    <meta property="og:description" content="Innovative portfolio showcasing AI projects and achievements.">
    <meta property="og:image" content="https://your-domain.com/og-image.jpg">
    <meta property="og:url" content="https://your-domain.com">
    <meta name="twitter:card" content="summary_large_image">
    <link rel="canonical" href="https://your-domain.com">
    <meta name="robots" content="index, follow">
    <title>Sachindra Shekhar Pandey - AI/ML Engineer & Space Tech Pioneer</title>
    <script async src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js" integrity="sha512-dZJFXkHGEjAIp4n0K0F0o4j68amz0ScZseIv+a5n4Tbn9UxxJllBv5V1QbDm2vumNL3p+pBvUpPJBV0AZw+JKg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html {
            scroll-behavior: smooth;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #000011;
            color: #ffffff;
            overflow-x: hidden;
            line-height: 1.6;
        }
        
        #space-canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
        }
        
        .container {
            position: relative;
            z-index: 1;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        .hero-section {
            text-align: center;
            padding: 100px 0;
            background: linear-gradient(45deg, rgba(0, 100, 255, 0.1), rgba(255, 0, 150, 0.1));
            backdrop-filter: blur(10px);
            border-radius: 20px;
            margin: 50px 0;
            border: 1px solid rgba(255, 255, 255, 0.1);
            animation: glow 3s ease-in-out infinite alternate;
        }
        
        @keyframes glow {
            from { box-shadow: 0 0 20px rgba(0, 100, 255, 0.3); }
            to { box-shadow: 0 0 40px rgba(255, 0, 150, 0.5), 0 0 60px rgba(0, 100, 255, 0.3); }
        }
        
        .hero-title {
            font-size: 4rem;
            font-weight: 700;
            background: linear-gradient(45deg, #00ffff, #ff00ff, #ffff00);
            background-size: 200% 200%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: rainbow 3s ease-in-out infinite;
            margin-bottom: 20px;
        }
        
        @keyframes rainbow {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }
        
        .hero-subtitle {
            font-size: 1.5rem;
            color: #00ffff;
            margin-bottom: 30px;
            text-shadow: 0 0 10px rgba(0, 255, 255, 0.5);
        }
        
        .contact-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 30px;
        }
        
        .contact-link {
            padding: 12px 25px;
            background: linear-gradient(45deg, rgba(0, 255, 255, 0.2), rgba(255, 0, 255, 0.2));
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 25px;
            color: white;
            text-decoration: none;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            min-width: 48px;
            min-height: 48px;
        }
        
        .contact-link:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 10px 25px rgba(0, 255, 255, 0.4);
            background: linear-gradient(45deg, rgba(0, 255, 255, 0.4), rgba(255, 0, 255, 0.4));
        }
        
        .section {
            margin: 50px 0;
            padding: 40px;
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.05), rgba(0, 0, 0, 0.1));
            border-radius: 15px;
            backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
            opacity: 0;
            transform: translateY(50px);
        }
        
        .section:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 255, 255, 0.2);
        }
        
        .section-title {
            font-size: 2.5rem;
            color: #00ffff;
            margin-bottom: 30px;
            text-align: center;
            position: relative;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: linear-gradient(45deg, #00ffff, #ff00ff);
            border-radius: 2px;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
        
        .skill-card {
            padding: 25px;
            background: linear-gradient(45deg, rgba(0, 100, 255, 0.1), rgba(255, 0, 150, 0.1));
            border-radius: 15px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.3s ease;
            text-align: center;
        }
        
        .skill-card:hover {
            transform: rotateY(5deg) scale(1.05);
            box-shadow: 0 15px 30px rgba(255, 0, 150, 0.3);
        }
        
        .skill-title {
            font-size: 1.3rem;
            color: #ff00ff;
            margin-bottom: 15px;
        }
        
        .experience-item {
            margin-bottom: 40px;
            padding: 30px;
            background: linear-gradient(135deg, rgba(0, 255, 255, 0.05), rgba(255, 0, 255, 0.05));
            border-left: 4px solid #00ffff;
            border-radius: 10px;
            transition: all 0.3s ease;
        }
        
        .experience-item:hover {
            transform: translateX(10px);
            box-shadow: -10px 0 30px rgba(0, 255, 255, 0.2);
        }
        
        .experience-title {
            font-size: 1.8rem;
            color: #00ffff;
            margin-bottom: 10px;
        }
        
        .experience-company {
            font-size: 1.2rem;
            color: #ff00ff;
            margin-bottom: 15px;
        }
        
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }
        
        .project-card {
            padding: 30px;
            background: linear-gradient(45deg, rgba(255, 255, 255, 0.05), rgba(0, 0, 0, 0.3));
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }
        
        .project-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent, rgba(0, 255, 255, 0.1), transparent);
            transform: rotate(45deg);
            transition: all 0.5s ease;
            opacity: 0;
        }
        
        .project-card:hover::before {
            opacity: 1;
            animation: shine 0.5s ease-in-out;
        }
        
        @keyframes shine {
            0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); }
            100% { transform: translateX(100%) translateY(100%) rotate(45deg); }
        }
        
        .project-card:hover {
            transform: translateY(-15px) rotateX(5deg);
            box-shadow: 0 25px 50px rgba(0, 255, 255, 0.3);
        }
        
        .project-title {
            font-size: 1.5rem;
            color: #00ffff;
            margin-bottom: 15px;
            position: relative;
            z-index: 2;
        }
        
        .project-link {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 20px;
            background: linear-gradient(45deg, #00ffff, #ff00ff);
            color: white;
            text-decoration: none;
            border-radius: 20px;
            font-weight: bold;
            transition: all 0.3s ease;
            position: relative;
            z-index: 2;
        }
        
        .project-link:hover {
            transform: scale(1.1);
            box-shadow: 0 5px 15px rgba(0, 255, 255, 0.5);
        }
        
        .achievements-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .achievement-card {
            padding: 25px;
            background: linear-gradient(135deg, rgba(255, 215, 0, 0.1), rgba(255, 0, 150, 0.1));
            border-radius: 15px;
            border: 2px solid rgba(255, 215, 0, 0.3);
            text-align: center;
            transition: all 0.3s ease;
            position: relative;
        }
        
        .achievement-card::before {
            content: '🏆';
            position: absolute;
            top: -15px;
            right: -15px;
            font-size: 2rem;
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }
        
        .achievement-card:hover {
            transform: scale(1.05) rotate(2deg);
            box-shadow: 0 15px 30px rgba(255, 215, 0, 0.4);
        }
        
        .stats-container {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin: 50px 0;
            gap: 20px;
        }
        
        .stat-item {
            text-align: center;
            padding: 20px;
            background: linear-gradient(45deg, rgba(0, 255, 255, 0.2), rgba(255, 0, 255, 0.2));
            border-radius: 15px;
            min-width: 150px;
        }
        
        .stat-number {
            font-size: 3rem;
            font-weight: bold;
            color: #00ffff;
            display: block;
        }
        
        .footer {
            text-align: center;
            padding: 50px;
            margin-top: 100px;
            background: linear-gradient(45deg, rgba(0, 0, 0, 0.8), rgba(0, 0, 50, 0.8));
            border-radius: 20px;
        }
        
        .typing-animation {
            border-right: 2px solid #00ffff;
            animation: blink 1s infinite;
        }
        
        @keyframes blink {
            0%, 50% { border-color: #00ffff; }
            51%, 100% { border-color: transparent; }
        }
        
        a:focus, .contact-link:focus, .project-card:focus-within {
            outline: 2px solid #00ffff;
            outline-offset: 2px;
        }
        
        @media (max-width: 768px) {
            .hero-title { font-size: 2.5rem; }
            .hero-subtitle { font-size: 1.2rem; }
            .section-title { font-size: 2rem; }
            .contact-links { flex-direction: column; align-items: center; }
            .project-grid, .skills-grid, .achievements-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <canvas id="space-canvas"></canvas>
    
    <div class="container">
        <!-- Hero Section -->
        <header class="hero-section" role="banner">
            <h1 class="hero-title">Sachindra Shekhar Pandey</h1>
            <p class="hero-subtitle">AI/ML Engineer • Backend Developer • Space Tech Pioneer <span class="typing-animation"></span></p>
            <p style="font-size: 1.1rem; margin: 20px 0; color: #ffffff; opacity: 0.9;">
                🚀 Google Agentic AI Hackathon Finalist | 🛰️ ISRO Bharatiya Antariksh Semi-Finalist | 🌟 Open Source Contributor
            </p>
            <p style="color: #00ffff; margin-bottom: 30px;">📍 Lucknow, UP, India • Open to Relocation & Visa Sponsorship • Remote Ready</p>
            
            <nav class="contact-links">
                <a href="tel:+917905604539" class="contact-link" aria-label="Call +91 79056 04539">📞 +91 79056 04539</a>
                <a href="mailto:sachindrapandey328@gmail.com" class="contact-link" aria-label="Email Sachindra Shekhar Pandey">✉️ Email</a>
                <a href="https://linkedin.com/in/sachindra-shekhar-pandey-73b45427b" class="contact-link" aria-label="LinkedIn Profile">💼 LinkedIn</a>
                <a href="https://github.com/Sachindrapandeyyy" class="contact-link" aria-label="GitHub Profile">🐱 GitHub</a>
            </nav>
        </header>

        <div class="stats-container">
            <div class="stat-item">
                <span class="stat-number">9000+</span>
                <span>Teams Competed Against</span>
            </div>
            <div class="stat-item">
                <span class="stat-number">600+</span>
                <span>Community Members</span>
            </div>
            <div class="stat-item">
                <span class="stat-number">1000+</span>
                <span>Users Supported</span>
            </div>
            <div class="stat-item">
                <span class="stat-number">95%</span>
                <span>Accuracy Achieved</span>
            </div>
        </div>

        <!-- Professional Summary -->
        <section class="section" role="region" aria-labelledby="professional-summary-title">
            <h2 class="section-title" id="professional-summary-title">🚀 Professional Summary</h2>
            <p style="font-size: 1.2rem; text-align: center; line-height: 1.8;">
                Motivated Computer Science undergraduate with strong foundation in <strong style="color: #00ffff;">AI/ML development</strong> and 
                <strong style="color: #ff00ff;">backend engineering</strong>. Google Agentic AI Hackathon <strong style="color: #ffff00;">Finalist</strong> 
                among 9,000+ global teams and Bharatiya Antariksh Hackathon <strong style="color: #00ffff;">Semi-Finalist</strong> with advanced 
                weather nowcasting system. Demonstrated expertise through impactful projects in machine learning, computer vision, 
                and scalable web applications with real-time analytics capabilities.
            </p>
        </section>

        <!-- Technical Skills -->
        <section class="section" role="region" aria-labelledby="technical-skills-title">
            <h2 class="section-title" id="technical-skills-title">⚡ Technical Arsenal</h2>
            <div class="skills-grid">
                <article class="skill-card">
                    <h3 class="skill-title">🐍 Programming Languages</h3>
                    <p>Python (Advanced, 3+ years), C++, Java, JavaScript, C# (.NET), SQL</p>
                </article>
                <article class="skill-card">
                    <h3 class="skill-title">🤖 AI/ML Technologies</h3>
                    <p>TensorFlow, PyTorch, Scikit-learn, OpenCV, Keras, Mediapipe, NumPy, Computer Vision, NLP, Diffusion Models</p>
                </article>
                <article class="skill-card">
                    <h3 class="skill-title">🚀 Backend & APIs</h3>
                    <p>FastAPI, Flask, Django, REST APIs, GraphQL, Microservices, JWT Authentication, API Gateway</p>
                </article>
                <article class="skill-card">
                    <h3 class="skill-title">☁️ Cloud & DevOps</h3>
                    <p>Google Cloud Platform (Vertex AI, Cloud Run, BigQuery), Azure, Firebase, Docker, Kubernetes, CI/CD</p>
                </article>
                <article class="skill-card">
                    <h3 class="skill-title">🗄️ Databases & Storage</h3>
                    <p>PostgreSQL, MySQL, MongoDB, Redis, Firebase Firestore, Vector Databases</p>
                </article>
                <article class="skill-card">
                    <h3 class="skill-title">🌟 Specialized Skills</h3>
                    <p>Latent Diffusion Models, VAE, UNet3D, Satellite Image Processing, Weather Data Analysis, Geospatial Computing</p>
                </article>
            </div>
        </section>

        <!-- Education -->
        <section class="section" role="region" aria-labelledby="education-title">
            <h2 class="section-title" id="education-title">🎓 Academic Excellence</h2>
            <article class="experience-item">
                <h3 class="experience-title">B.Tech Computer Science & Engineering</h3>
                <p class="experience-company">Shri Ramswaroop Memorial University, Lucknow</p>
                <p style="color: #00ffff; margin-bottom: 15px;">📅 Aug 2022 – May 2026</p>
                <p><strong>Relevant Coursework:</strong> Data Structures & Algorithms, Database Management Systems, Machine Learning, 
                Deep Learning, Software Engineering, Computer Networks, System Design, Cloud Computing, Artificial Intelligence</p>
                
                <h4 style="color: #ff00ff; margin-top: 20px;">📚 Research Publications & Technical Writing:</h4>
                <ul style="margin-top: 10px; color: #ffffff;">
                    <li>"Why Traditional Programming Skills Are No Longer the Gatekeepers of AI Innovation"</li>
                    <li>"Project Bhasha Setu: Bridging Language Barriers with Multilingual AI"</li>
                    <li>"Project Chakshu: Advanced Weather Nowcasting using Latent Diffusion Models"</li>
                    <li>"Privacy-Preserving Machine Learning: Implementation and Challenges"</li>
                </ul>
            </article>
        </section>

        <!-- Professional Experience -->
        <section class="section" role="region" aria-labelledby="professional-journey-title">
            <h2 class="section-title" id="professional-journey-title">💼 Professional Journey</h2>
            
            <article class="experience-item">
                <h3 class="experience-title">Software Engineering Intern</h3>
                <p class="experience-company">NTPC Limited (Fortune 500 Energy Company) • Shaktinagar, UP</p>
                <p style="color: #00ffff; margin-bottom: 15px;">📅 Jun 2025 – Jul 2025</p>
                <ul style="color: #ffffff;">
                    <li>🏗️ Architected comprehensive secure legal document management system using Flask + PostgreSQL</li>
                    <li>⚡ Achieved <strong style="color: #00ffff;">30% reduction in document retrieval time</strong> through intelligent caching strategies</li>
                    <li>🔧 Built automated workflow engines using C#/.NET, improving system scalability by <strong style="color: #ff00ff;">20%</strong></li>
                    <li>📊 Enhanced enterprise dashboards for 200+ users, increasing satisfaction by <strong style="color: #ffff00;">25%</strong></li>
                    <li>⏰ Eliminated 40+ hours of manual processing work weekly through automation</li>
                    <li>🎯 Maintained <strong style="color: #00ffff;">99.9% system uptime</strong> with comprehensive monitoring</li>
                </ul>
            </article>
            
            <article class="experience-item">
                <h3 class="experience-title">Software Developer Intern</h3>
                <p class="experience-company">Skillzee (EdTech Startup) • Remote</p>
                <p style="color: #00ffff; margin-bottom: 15px;">📅 Dec 2023 – Jan 2024</p>
                <ul style="color: #ffffff;">
                    <li>🚀 Enhanced user onboarding completion rate by <strong style="color: #00ffff;">15%</strong> through UX optimization</li>
                    <li>🔗 Developed robust RESTful API infrastructure supporting <strong style="color: #ff00ff;">1000+ concurrent users</strong></li>
                    <li>🧪 Implemented comprehensive testing framework, reducing production bugs by <strong style="color: #ffff00;">25%</strong></li>
                    <li>⚡ Delivered features <strong style="color: #00ffff;">10% faster</strong> through improved agile processes</li>
                    <li>📈 Optimized API response times and resource management for scalability</li>
                </ul>
            </article>
        </section>

        <!-- Featured Projects -->
        <section class="section" role="region" aria-labelledby="featured-projects-title">
            <h2 class="section-title" id="featured-projects-title">🌟 Featured Projects & Innovations</h2>
            <div class="project-grid">
                
                <article class="project-card">
                    <h3 class="project-title">🛰️ Project Chakshu - AI Weather Nowcasting</h3>
                    <p style="margin-bottom: 15px; color: #ffff00; font-weight: bold;">🏆 Bharatiya Antariksh Hackathon 2025 Semi-Finalist</p>
                    <p>Revolutionary weather prediction platform utilizing INSAT satellite imagery and cutting-edge latent-space diffusion models. 
                    Developed sophisticated VAE + UNet3D architecture with complexity conditioning algorithms for precise 0-6 hour weather forecasts.</p>
                    <p style="margin-top: 15px; color: #00ffff;"><strong>Tech Stack:</strong> PyTorch, Computer Vision, Satellite Data Processing, Advanced Diffusion Models</p>
                    <p style="color: #ff00ff;"><strong>Achievements:</strong> SSIM >0.8, CSI >0.7 for critical weather events, 2-3 second inference time</p>
                    <a href="https://github.com/Sachindrapandeyyy" class="project-link">🚀 View Project</a>
                </article>
                
                <article class="project-card">
                    <h3 class="project-title">👥 Project Drishti - AI Crowd Management</h3>
                    <p style="margin-bottom: 15px; color: #ffff00; font-weight: bold;">🏆 Google Agentic AI Hackathon Featured</p>
                    <p>Comprehensive backend infrastructure using FastAPI + Firebase + Google Cloud Vertex AI for real-time crowd analytics 
                    supporting large-scale event management with ML pipeline for crowd density prediction and emergency detection.</p>
                    <p style="margin-top: 15px; color: #00ffff;"><strong>Tech Stack:</strong> FastAPI, Computer Vision, Firebase, Google Cloud Platform, Microservices</p>
                    <p style="color: #ff00ff;"><strong>Impact:</strong> Sub-3s latency, 50k+ attendee event support, Real-time analytics</p>
                    <a href="https://github.com/Sachindrapandeyyy" class="project-link">💻 GitHub</a>
                </article>
                
                <article class="project-card">
                    <h3 class="project-title">🏙️ UrbanSync - Smart City Platform</h3>
                    <p style="margin-bottom: 15px; color: #ffff00; font-weight: bold;">🌍 IBM Call for Code Initiative</p>
                    <p>Comprehensive urban management solution featuring advanced air quality monitoring algorithms, predictive traffic analysis models, 
                    and integrated disaster response mapping systems with end-to-end ML pipeline.</p>
                    <p style="margin-top: 15px; color: #00ffff;"><strong>Tech Stack:</strong> Python, TensorFlow, MongoDB, REST APIs, Data Analytics</p>
                    <p style="color: #ff00ff;"><strong>Features:</strong> Real-time dashboard, Urban planning algorithms, Policy maker tools</p>
                    <a href="https://github.com/Sachindrapandeyyy" class="project-link">🌐 View Demo</a>
                </article>
                
                <article class="project-card">
                    <h3 class="project-title">🔒 NSS Secure Data Platform</h3>
                    <p style="margin-bottom: 15px; color: #ffff00; font-weight: bold;">🛡️ Statathon 2025 Featured</p>
                    <p>Enterprise-grade secure data processing platform implementing advanced k-anonymity and differential privacy algorithms 
                    for GDPR-compliant machine learning operations while maintaining optimal model accuracy.</p>
                    <p style="margin-top: 15px; color: #00ffff;"><strong>Tech Stack:</strong> Python, Advanced Cryptography, Privacy Engineering, FastAPI</p>
                    <p style="color: #ff00ff;"><strong>Innovation:</strong> Data anonymization, Regulatory compliance, Enterprise security</p>
                    <a href="https://github.com/Sachindrapandeyyy" class="project-link">🔐 Explore</a>
                </article>
                
                <article class="project-card">
                    <h3 class="project-title">🤖 Edith - AI Personal Assistant</h3>
                    <p>Sophisticated multi-modal AI assistant leveraging advanced NLP and intelligent API orchestration, processing 100+ daily queries 
                    with context-aware response generation and comprehensive automation suite.</p>
                    <p style="margin-top: 15px; color: #00ffff;"><strong>Tech Stack:</strong> Python, Advanced NLP, API Integration, Voice Recognition</p>
                    <p style="color: #ff00ff;"><strong>Capabilities:</strong> 90% accuracy, Task automation, Voice commands, Email management</p>
                    <a href="https://github.com/Sachindrapandeyyy" class="project-link">🎯 Try It</a>
                </article>
                
                <article class="project-card">
                    <h3 class="project-title">🎮 Kill Diptera - CV Gaming Engine</h3>
                    <p>Innovative gesture-controlled gaming system using advanced MediaPipe and OpenCV frameworks, achieving 95% gesture 
                    recognition accuracy at 30+ FPS with sophisticated real-time hand tracking algorithms.</p>
                    <p style="margin-top: 15px; color: #00ffff;"><strong>Tech Stack:</strong> Python, OpenCV, Mediapipe, Computer Vision</p>
                    <p style="color: #ff00ff;"><strong>Performance:</strong> 95% accuracy, 30+ FPS, Real-time tracking, Collision detection</p>
                    <a href="https://github.com/Sachindrapandeyyy" class="project-link">🕹️ Play Game</a>
                </article>
            </div>
        </section>

        <!-- Achievements & Recognition -->
        <section class="section" role="region" aria-labelledby="achievements-title">
            <h2 class="section-title" id="achievements-title">🏆 Achievements & Recognition</h2>
            <div class="achievements-grid">
                <article class="achievement-card">
                    <h3 style="color: #ffff00;">🥇 Google Agentic AI Hackathon Finalist</h3>
                    <p>Selected from <strong style="color: #00ffff;">9,000+ global participants</strong> (Top 0.1%)</p>
                    <p>Built sophisticated AI agent for automated task management with intelligent workflow optimization</p>
                </article>
                
                <article class="achievement-card">
                    <h3 style="color: #ffff00;">🛰️ ISRO Bharatiya Antariksh Semi-Finalist</h3>
                    <p>Advanced weather nowcasting system using <strong style="color: #ff00ff;">cutting-edge diffusion models</strong></p>
                    <p>Revolutionary AI-powered weather prediction for Indian meteorological patterns</p>
                </article>
                
                <article class="achievement-card">
                    <h3 style="color: #ffff00;">🌍 Open Source Contributor</h3>
                    <p><strong style="color: #00ffff;">Project Bhasha Setu</strong> - Multilingual AI translation modules</p>
                    <p>Enhanced accessibility and global reach of AI-powered language processing</p>
                </article>
                
                <article class="achievement-card">
                    <h3 style="color: #ffff00;">👥 Community Founder & Leader</h3>
                    <p><strong style="color: #ff00ff;">Developer Community SRMU</strong> - 600+ active members</p>
                    <p>Organized multiple hackathons, coding workshops, and networking events</p>
                </article>
                
                <article class="achievement-card">
                    <h3 style="color: #ffff00;">📋 Event Coordinator</h3>
                    <p><strong style="color: #00ffff;">Smart India Hackathon</strong> - 300+ participants</p>
                    <p>Successfully coordinated large-scale national hackathon with team formation processes</p>
                </article>
                
                <article class="achievement-card">
                    <h3 style="color: #ffff00;">🎓 Technical Mentor</h3>
                    <p>Guided <strong style="color: #ff00ff;">20+ students</strong> in programming and career development</p>
                    <p>Helped students secure internships and improve technical skills through structured guidance</p>
                </article>
            </div>
        </section>

        <!-- Certifications & Professional Development -->
        <section class="section" role="region" aria-labelledby="certifications-title">
            <h2 class="section-title" id="certifications-title">📜 Certifications & Professional Development</h2>
            <div class="skills-grid">
                <article class="skill-card">
                    <h3 class="skill-title">🎯 Completed Certifications</h3>
                    <p><strong style="color: #00ffff;">Quantum Computing Certificate</strong> (Udemy)</p>
                    <p><strong style="color: #ff00ff;">Artificial Intelligence Certificate</strong> (L&T EduTech)</p>
                    <p><strong style="color: #ffff00;">Deep Learning Specialization</strong> (Coursera)</p>
                </article>
                <article class="skill-card">
                    <h3 class="skill-title">🚀 In Progress</h3>
                    <p><strong style="color: #00ffff;">Google Cloud Associate Engineer</strong></p>
                    <p><strong style="color: #ff00ff;">MongoDB Certified Developer</strong></p>
                    <p><strong style="color: #ffff00;">Advanced Cloud Architecture</strong></p>
                </article>
                <article class="skill-card">
                    <h3 class="skill-title">💡 Specialized Training</h3>
                    <p>Computer Vision Fundamentals</p>
                    <p>Microservices Design Patterns</p>
                    <p>Technical Leadership Workshop</p>
                    <p>Agile Project Management</p>
                </article>
            </div>
        </section>

        <!-- Leadership & Impact -->
        <section class="section" role="region" aria-labelledby="leadership-title">
            <h2 class="section-title" id="leadership-title">🎯 Leadership & Community Impact</h2>
            <article class="experience-item">
                <h3 class="experience-title">🚀 Developer Community SRMU - Founder & Leader</h3>
                <p style="color: #00ffff; margin-bottom: 15px;">📊 Grew to 600+ Active Members</p>
                <ul style="color: #ffffff;">
                    <li>🎯 Established and led thriving developer community from ground zero</li>
                    <li>📅 Organized 15+ technical hackathons, coding workshops, and networking events</li>
                    <li>🌟 Created structured mentorship programs for emerging developers</li>
                    <li>💡 Facilitated collaboration between students and industry professionals</li>
                    <li>📈 Achieved 85% member engagement rate through innovative programming</li>
                </ul>
            </article>
            
            <article class="experience-item">
                <h3 class="experience-title">🏆 Smart India Hackathon 2024 - Campus Coordinator</h3>
                <p style="color: #00ffff; margin-bottom: 15px;">👥 300+ Participants Managed</p>
                <ul style="color: #ffffff;">
                    <li>🎪 Successfully coordinated large-scale national hackathon event</li>
                    <li>🤝 Facilitated team formation processes and mentor assignments</li>
                    <li>📋 Managed logistics, registration, and technical infrastructure</li>
                    <li>🎯 Achieved 95% participant satisfaction rating</li>
                    <li>🏅 Recognized by organizing committee for exceptional coordination</li>
                </ul>
            </article>
            
            <article class="experience-item">
                <h3 class="experience-title">👨‍🏫 Technical Mentor & Career Guide</h3>
                <p style="color: #00ffff; margin-bottom: 15px;">🎓 20+ Students Mentored Successfully</p>
                <ul style="color: #ffffff;">
                    <li>💼 Helped students secure internships at top tech companies</li>
                    <li>📚 Provided structured guidance in programming and system design</li>
                    <li>🎯 Conducted mock interviews and technical skill assessments</li>
                    <li>📈 Achieved 80% success rate in student placement outcomes</li>
                    <li>🌟 Received outstanding mentor recognition from university</li>
                </ul>
            </article>
        </section>

        <!-- Technologies in Action -->
        <section class="section" role="region" aria-labelledby="technology-stack-title">
            <h2 class="section-title" id="technology-stack-title">⚙️ Technology Stack Deep Dive</h2>
            <div class="project-grid">
                <article class="project-card">
                    <h3 class="project-title">🧠 AI/ML Expertise</h3>
                    <p><strong style="color: #00ffff;">Advanced Models:</strong> Latent Diffusion Models, VAE, UNet3D, Transformer Architectures</p>
                    <p><strong style="color: #ff00ff;">Computer Vision:</strong> OpenCV, Mediapipe, Image Processing, Object Detection, Gesture Recognition</p>
                    <p><strong style="color: #ffff00;">NLP:</strong> Text Processing, Sentiment Analysis, Language Models, Multi-lingual AI</p>
                    <p><strong style="color: #00ffff;">Specialized:</strong> Weather Data Analysis, Satellite Image Processing, Geospatial Computing</p>
                </article>
                
                <article class="project-card">
                    <h3 class="project-title">🏗️ Backend Architecture</h3>
                    <p><strong style="color: #00ffff;">APIs:</strong> FastAPI, Flask, Django, REST, GraphQL, Microservices</p>
                    <p><strong style="color: #ff00ff;">Authentication:</strong> JWT, OAuth, Role-based Access Control, Security Best Practices</p>
                    <p><strong style="color: #ffff00;">Performance:</strong> Caching Strategies, Database Optimization, Load Balancing</p>
                    <p><strong style="color: #00ffff;">Testing:</strong> Unit Tests, Integration Testing, End-to-End Validation</p>
                </article>
                
                <article class="project-card">
                    <h3 class="project-title">☁️ Cloud & DevOps</h3>
                    <p><strong style="color: #00ffff;">Google Cloud:</strong> Vertex AI, Cloud Run, BigQuery, Firebase, Cloud Functions</p>
                    <p><strong style="color: #ff00ff;">Azure:</strong> ML Studio, App Services, Cognitive Services, Storage Solutions</p>
                    <p><strong style="color: #ffff00;">DevOps:</strong> Docker, Kubernetes, CI/CD Pipelines, Infrastructure as Code</p>
                    <p><strong style="color: #00ffff;">Monitoring:</strong> Logging, Error Tracking, Performance Monitoring, Alerting</p>
                </article>
            </div>
        </section>

        <!-- Research & Publications -->
        <section class="section" role="region" aria-labelledby="research-title">
            <h2 class="section-title" id="research-title">📖 Research & Technical Publications</h2>
            
            <article class="experience-item">
                <h3 class="experience-title">📝 "Why Traditional Programming Skills Are No Longer the Gatekeepers of AI Innovation"</h3>
                <p style="color: #00ffff; margin-bottom: 15px;">Technical Analysis on AI Democratization</p>
                <p>Comprehensive analysis of how no-code AI platforms are reshaping the innovation landscape, democratizing access to 
                artificial intelligence development, and reducing barriers for non-traditional programmers to contribute to AI advancement.</p>
            </article>
            
            <article class="experience-item">
                <h3 class="experience-title">🌐 "Project Bhasha Setu: Bridging Language Barriers with Multilingual AI"</h3>
                <p style="color: #00ffff; margin-bottom: 15px;">Open Source Research Contribution</p>
                <p>Research paper detailing the development of multilingual AI translation modules that enable seamless cross-language 
                communication, focusing on Indian regional languages and accessibility improvements for diverse user bases.</p>
            </article>
            
            <article class="experience-item">
                <h3 class="experience-title">🛰️ "Project Chakshu: Advanced Weather Nowcasting using Latent Diffusion Models"</h3>
                <p style="color: #00ffff; margin-bottom: 15px;">Space Technology Research Paper</p>
                <p>Detailed technical documentation of revolutionary weather prediction system utilizing INSAT satellite imagery and 
                cutting-edge latent diffusion models, specifically optimized for Indian meteorological patterns and short-term forecasting accuracy.</p>
            </article>
            
            <article class="experience-item">
                <h3 class="experience-title">🔒 "Privacy-Preserving Machine Learning: Implementation and Challenges"</h3>
                <p style="color: #00ffff; margin-bottom: 15px;">Data Security Research Documentation</p>
                <p>Comprehensive study on implementing privacy-preserving techniques in machine learning systems, focusing on 
                k-anonymity, differential privacy, and GDPR compliance while maintaining model accuracy and performance.</p>
            </article>
        </section>

        <!-- Current Focus & Future Vision -->
        <section class="section" role="region" aria-labelledby="current-focus-title">
            <h2 class="section-title" id="current-focus-title">🔮 Current Focus & Future Vision</h2>
            <div class="skills-grid">
                <article class="skill-card">
                    <h3 class="skill-title">🎯 Current Research Areas</h3>
                    <p><strong style="color: #00ffff;">AI for Climate Science:</strong> Advanced weather prediction models</p>
                    <p><strong style="color: #ff00ff;">Edge Computing:</strong> Optimizing AI inference on resource-constrained devices</p>
                    <p><strong style="color: #ffff00;">Privacy-Preserving AI:</strong> Secure machine learning implementations</p>
                </article>
                
                <article class="skill-card">
                    <h3 class="skill-title">🚀 Future Goals</h3>
                    <p><strong style="color: #00ffff;">Quantum Machine Learning:</strong> Exploring quantum-enhanced AI algorithms</p>
                    <p><strong style="color: #ff00ff;">Space Technology:</strong> AI applications for satellite data processing</p>
                    <p><strong style="color: #ffff00;">Sustainable AI:</strong> Energy-efficient machine learning solutions</p>
                </article>
                
                <article class="skill-card">
                    <h3 class="skill-title">🌟 Innovation Areas</h3>
                    <p><strong style="color: #00ffff;">Multimodal AI:</strong> Integrating vision, language, and audio processing</p>
                    <p><strong style="color: #ff00ff;">Autonomous Systems:</strong> Self-learning and adaptive AI architectures</p>
                    <p><strong style="color: #ffff00;">Human-AI Collaboration:</strong> Intuitive interfaces for AI interaction</p>
                </article>
            </div>
        </section>

        <!-- Professional References -->
        <section class="section" role="region" aria-labelledby="professional-recognition-title">
            <h2 class="section-title" id="professional-recognition-title">✨ Professional Recognition</h2>
            <div class="achievements-grid">
                <article class="achievement-card">
                    <h3 style="color: #ffff00;">📋 Letters of Recommendation</h3>
                    <p><strong style="color: #00ffff;">HP India:</strong> Exceptional technical contributions and leadership capabilities</p>
                    <p><strong style="color: #ff00ff;">Skillzee:</strong> Outstanding performance and professional development potential</p>
                </article>
                
                <article class="achievement-card">
                    <h3 style="color: #ffff00;">🏢 Industry Recognition</h3>
                    <p><strong style="color: #00ffff;">NTPC Limited:</strong> System architecture excellence and innovation</p>
                    <p><strong style="color: #ff00ff;">University Faculty:</strong> Outstanding academic performance and research contributions</p>
                </article>
            </div>
        </section>

        <!-- Contact & Availability -->
        <section class="section" role="region" aria-labelledby="connect-title">
            <h2 class="section-title" id="connect-title">🤝 Let's Connect & Collaborate</h2>
            <div style="text-align: center; margin: 40px 0;">
                <p style="font-size: 1.3rem; color: #00ffff; margin-bottom: 20px;">
                    🚀 Ready for New Challenges • Open to Full-Time Opportunities
                </p>
                <p style="font-size: 1.1rem; color: #ffffff; margin-bottom: 30px;">
                    ✈️ Open to Relocation & Visa Sponsorship • 🌍 Remote Work Ready • 📅 Immediate Availability
                </p>
                
                <div style="display: flex; justify-content: space-around; flex-wrap: wrap; gap: 20px; margin-top: 30px;">
                    <div style="padding: 20px; background: linear-gradient(45deg, rgba(0, 255, 255, 0.1), rgba(255, 0, 255, 0.1)); border-radius: 15px; min-width: 200px;">
                        <h4 style="color: #00ffff; margin-bottom: 10px;">🎯 Seeking Roles In</h4>
                        <p>AI/ML Engineer</p>
                        <p>Backend Developer</p>
                        <p>Full-Stack Developer</p>
                        <p>Data Scientist</p>
                    </div>
                    
                    <div style="padding: 20px; background: linear-gradient(45deg, rgba(255, 0, 150, 0.1), rgba(255, 215, 0, 0.1)); border-radius: 15px; min-width: 200px;">
                        <h4 style="color: #ff00ff; margin-bottom: 10px;">🌟 Preferred Industries</h4>
                        <p>Space Technology</p>
                        <p>Climate Tech</p>
                        <p>FinTech</p>
                        <p>Healthcare AI</p>
                    </div>
                    
                    <div style="padding: 20px; background: linear-gradient(45deg, rgba(255, 215, 0, 0.1), rgba(0, 255, 255, 0.1)); border-radius: 15px; min-width: 200px;">
                        <h4 style="color: #ffff00; margin-bottom: 10px;">💡 Collaboration Areas</h4>
                        <p>Open Source Projects</p>
                        <p>Research Initiatives</p>
                        <p>Hackathon Teams</p>
                        <p>Technical Mentoring</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="footer" role="contentinfo">
            <h2 style="color: #00ffff; margin-bottom: 20px;">🚀 "Building the Future, One Algorithm at a Time"</h2>
            <p style="font-size: 1.2rem; color: #ffffff; margin-bottom: 30px;">
                Passionate about leveraging <strong style="color: #ff00ff;">Artificial Intelligence</strong> and 
                <strong style="color: #00ffff;">Space Technology</strong> to solve real-world challenges and create 
                innovative solutions that make a meaningful impact on society.
            </p>
            
            <div style="display: flex; justify-content: center; gap: 30px; flex-wrap: wrap; margin: 30px 0;">
                <a href="tel:+917905604539" style="color: #00ffff; text-decoration: none; font-size: 1.1rem;">
                    📞 +91 79056 04539
                </a>
                <a href="mailto:sachindrapandey328@gmail.com" style="color: #ff00ff; text-decoration: none; font-size: 1.1rem;">
                    ✉️ sachindrapandey328@gmail.com
                </a>
                <a href="https://linkedin.com/in/sachindra-shekhar-pandey-73b45427b" style="color: #ffff00; text-decoration: none; font-size: 1.1rem;">
                    💼 LinkedIn Profile
                </a>
                <a href="https://github.com/Sachindrapandeyyy" style="color: #00ffff; text-decoration: none; font-size: 1.1rem;">
                    🐱 GitHub Portfolio
                </a>
            </div>
            
            <p style="color: #888; margin-top: 40px; font-size: 0.9rem;">
                ⭐ If you found this profile interesting, please consider starring some of my repositories!<br>
                🤝 Always open to discussing innovative ideas and potential collaborations.
            </p>
            
            <div style="margin-top: 30px; padding: 20px; background: linear-gradient(45deg, rgba(0, 0, 0, 0.3), rgba(0, 50, 100, 0.3)); border-radius: 15px;">
                <p style="color: #00ffff; font-size: 1.1rem; margin-bottom: 10px;">"Innovation is not about having all the answers,</p>
                <p style="color: #ff00ff; font-size: 1.1rem; margin-bottom: 10px;">it's about asking the right questions</p>
                <p style="color: #ffff00; font-size: 1.1rem;">and having the courage to explore the unknown."</p>
                <p style="color: #ffffff; margin-top: 15px; font-style: italic;">- Sachindra Shekhar Pandey</p>
            </div>
        </footer>
    </div>

    <script>
        // Three.js Space Animation
        let scene, camera, renderer, stars = [];
        let planets = [];
        let mouseX = 0, mouseY = 0;
        
        function init() {
            try {
                scene = new THREE.Scene();
                camera = new THREE.PerspectiveCamera(75, window.innerWidth / window.innerHeight, 0.1, 1000);
                renderer = new THREE.WebGLRenderer({ canvas: document.getElementById('space-canvas'), alpha: true });
                renderer.setSize(window.innerWidth, window.innerHeight);
                renderer.setClearColor(0x000011, 0.8);
                renderer.setPixelRatio(window.devicePixelRatio);
                
                // Create stars
                const starGeometry = new THREE.BufferGeometry();
                const starMaterial = new THREE.PointsMaterial({
                    color: 0xffffff,
                    size: 2,
                    transparent: true,
                    opacity: 0.8
                });
                
                const starVertices = new Float32Array(1500 * 3);
                for (let i = 0; i < 1500 * 3; i += 3) {
                    starVertices[i] = (Math.random() - 0.5) * 2000;
                    starVertices[i + 1] = (Math.random() - 0.5) * 2000;
                    starVertices[i + 2] = (Math.random() - 0.5) * 2000;
                }
                
                starGeometry.setAttribute('position', new THREE.BufferAttribute(starVertices, 3));
                const starField = new THREE.Points(starGeometry, starMaterial);
                scene.add(starField);
                
                // Create animated planets
                createPlanets();
                
                // Create nebula effect
                createNebula();
                
                camera.position.z = 5;
                
                // Mouse movement listener
                document.addEventListener('mousemove', onMouseMove, false);
                window.addEventListener('resize', onWindowResize, false);
            } catch (e) {
                console.error('Three.js initialization failed:', e);
            }
        }
        
        function createPlanets() {
            const planetData = [
                { size: 0.5, color: 0x00ffff, distance: 10, speed: 0.01 },
                { size: 0.3, color: 0xff00ff, distance: 15, speed: 0.008 },
                { size: 0.4, color: 0xffff00, distance: 20, speed: 0.006 },
                { size: 0.2, color: 0xff0080, distance: 25, speed: 0.004 }
            ];
            
            planetData.forEach((data, index) => {
                const geometry = new THREE.SphereGeometry(data.size, 32, 32);
                const material = new THREE.MeshBasicMaterial({ 
                    color: data.color,
                    transparent: true,
                    opacity: 0.7
                });
                const planet = new THREE.Mesh(geometry, material);
                
                planet.userData = {
                    distance: data.distance,
                    speed: data.speed,
                    angle: index * Math.PI / 2
                };
                
                scene.add(planet);
                planets.push(planet);
            });
        }
        
        function createNebula() {
            const nebulaGeometry = new THREE.PlaneGeometry(50, 50);
            const nebulaMaterial = new THREE.MeshBasicMaterial({
                color: 0x4406aa,
                transparent: true,
                opacity: 0.1,
                side: THREE.DoubleSide
            });
            
            for (let i = 0; i < 3; i++) {
                const nebula = new THREE.Mesh(nebulaGeometry, nebulaMaterial);
                nebula.position.set(
                    (Math.random() - 0.5) * 100,
                    (Math.random() - 0.5) * 100,
                    (Math.random() - 0.5) * 100
                );
                nebula.rotation.set(
                    Math.random() * Math.PI,
                    Math.random() * Math.PI,
                    Math.random() * Math.PI
                );
                scene.add(nebula);
            }
        }
        
        function onMouseMove(event) {
            mouseX = (event.clientX / window.innerWidth) * 2 - 1;
            mouseY = -(event.clientY / window.innerHeight) * 2 + 1;
        }
        
        function onWindowResize() {
            camera.aspect = window.innerWidth / window.innerHeight;
            camera.updateProjectionMatrix();
            renderer.setSize(window.innerWidth, window.innerHeight);
        }
        
        let lastTime = 0;
        const fps = 30;
        function animate(time) {
            try {
                requestAnimationFrame(animate);
                if (time - lastTime < 1000 / fps) return;
                lastTime = time;
                
                // Rotate planets
                planets.forEach(planet => {
                    planet.userData.angle += planet.userData.speed;
                    planet.position.x = Math.cos(planet.userData.angle) * planet.userData.distance;
                    planet.position.z = Math.sin(planet.userData.angle) * planet.userData.distance;
                    planet.rotation.y += 0.02;
                });
                
                // Camera movement based on mouse
                camera.position.x += (mouseX * 2 - camera.position.x) * 0.02;
                camera.position.y += (mouseY * 2 - camera.position.y) * 0.02;
                camera.lookAt(scene.position);
                
                // Rotate star field slowly
                scene.rotation.y += 0.0005;
                
                renderer.render(scene, camera);
            } catch (e) {
                console.error('Animation error:', e);
            }
        }
        
        // Scroll animations
        function handleScroll() {
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                const scroll = window.pageYOffset;
                const windowHeight = window.innerHeight;
                
                if (scroll > sectionTop - windowHeight + sectionHeight / 4) {
                    section.style.opacity = '1';
                    section.style.transform = 'translateY(0)';
                }
            });
        }
        
        // Particle cursor effect
        function createParticleCursor() {
            const particles = [];
            
            document.addEventListener('mousemove', (e) => {
                const particle = document.createElement('div');
                particle.style.position = 'fixed';
                particle.style.left = e.clientX + 'px';
                particle.style.top = e.clientY + 'px';
                particle.style.width = '4px';
                particle.style.height = '4px';
                particle.style.background = '#00ffff';
                particle.style.borderRadius = '50%';
                particle.style.pointerEvents = 'none';
                particle.style.opacity = '0.8';
                particle.style.zIndex = '9999';
                document.body.appendChild(particle);
                
                particles.push(particle);
                
                setTimeout(() => {
                    particle.style.opacity = '0';
                    setTimeout(() => {
                        document.body.removeChild(particle);
                        const index = particles.indexOf(particle);
                        if (index > -1) particles.splice(index, 1);
                    }, 300);
                }, 100);
                
                // Limit particles
                if (particles.length > 50) {
                    const oldParticle = particles.shift();
                    if (oldParticle) oldParticle.remove();
                }
            });
        }
        
        // Initialize everything
        window.addEventListener('load', () => {
            init();
            animate(performance.now());
            handleScroll();
            createParticleCursor();
            
            // Set initial styles for animations
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => {
                section.style.transition = 'all 0.8s ease';
            });
            
            // Typing animation for hero
            const typingElement = document.querySelector('.typing-animation');
            if (typingElement) {
                setTimeout(() => {
                    typingElement.style.borderRight = 'none';
                }, 3000);
            }
        });
        
        window.addEventListener('scroll', handleScroll);
        
        // Add some interactive elements
        document.querySelectorAll('.project-card, .skill-card, .achievement-card').forEach(card => {
            card.addEventListener('mouseenter', () => {
                card.style.transform = card.style.transform + ' scale(1.02)';
            });
            
            card.addEventListener('mouseleave', () => {
                card.style.transform = card.style.transform.replace(' scale(1.02)', '');
            });
        });
    </script>
</body>
</html>
