<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shantanu Pundir - Android Developer</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            animation: fadeInUp 0.8s ease-out;
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

        .header {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }

        .profile-name {
            font-size: 3rem;
            font-weight: 700;
            background: linear-gradient(45deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 10px;
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { filter: brightness(1); }
            to { filter: brightness(1.2); }
        }

        .tagline {
            font-size: 1.2rem;
            color: #666;
            margin-bottom: 20px;
        }

        .emoji {
            font-size: 1.5rem;
            display: inline-block;
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
            40% { transform: translateY(-10px); }
            60% { transform: translateY(-5px); }
        }

        .description {
            font-size: 1.1rem;
            color: #555;
            margin-bottom: 40px;
            text-align: center;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .section {
            margin-bottom: 35px;
            opacity: 0;
            animation: slideIn 0.6s ease-out forwards;
        }

        .section:nth-child(2) { animation-delay: 0.2s; }
        .section:nth-child(3) { animation-delay: 0.4s; }
        .section:nth-child(4) { animation-delay: 0.6s; }

        @keyframes slideIn {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .section-title {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 15px;
            color: #4a5568;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-bottom: 30px;
        }

        .tech-category {
            background: linear-gradient(135deg, #f7fafc 0%, #edf2f7 100%);
            padding: 20px;
            border-radius: 15px;
            border-left: 4px solid #667eea;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .tech-category:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }

        .category-title {
            font-weight: 600;
            color: #2d3748;
            margin-bottom: 10px;
            font-size: 1.1rem;
        }

        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .skill-tag {
            background: linear-gradient(45deg, #667eea, #764ba2);
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
            transition: transform 0.2s ease;
        }

        .skill-tag:hover {
            transform: scale(1.05);
            cursor: pointer;
        }

        .stats-placeholder {
            text-align: center;
            padding: 30px;
            background: linear-gradient(135deg, #e2e8f0 0%, #cbd5e0 100%);
            border-radius: 15px;
            margin: 20px 0;
            border: 2px dashed #a0aec0;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .contact-item {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 20px;
            border-radius: 15px;
            text-decoration: none;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            display: flex;
            align-items: center;
            gap: 15px;
            font-weight: 500;
        }

        .contact-item:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(102, 126, 234, 0.3);
            color: white;
            text-decoration: none;
        }

        .contact-icon {
            font-size: 1.5rem;
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .wave {
            animation: wave 0.6s ease-in-out infinite;
        }

        @keyframes wave {
            0%, 100% { transform: rotate(0deg); }
            25% { transform: rotate(20deg); }
            75% { transform: rotate(-10deg); }
        }

        @media (max-width: 768px) {
            .container {
                padding: 20px;
                margin: 10px;
            }
            
            .profile-name {
                font-size: 2rem;
            }
            
            .tech-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Particle background animation */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: rgba(255, 255, 255, 0.5);
            border-radius: 50%;
            animation: float 6s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); opacity: 1; }
            50% { transform: translateY(-20px) rotate(180deg); opacity: 0.5; }
        }
    </style>
</head>
<body>
    <div class="particles"></div>
    
    <div class="container">
        <div class="header">
            <h1 class="profile-name">
                <span class="emoji wave">👋</span> Hi, I'm Shantanu Pundir
            </h1>
            <div class="tagline">
                <span class="emoji">🚀</span> Android Developer | 
                <span class="emoji">💻</span> Programmer | 
                <span class="emoji">📱</span> Tech Enthusiast
            </div>
        </div>

        <div class="description">
            I'm passionate about Android app development and love building applications that provide real value to users. 
            With strong foundations in Java, Kotlin, Python, JavaScript, and hands-on experience with modern Android 
            tools & architectures, I aim to craft clean, efficient, and scalable solutions.
        </div>

        <div class="section">
            <h2 class="section-title">
                <span class="emoji">🔧</span> Tech Stack & Skills
            </h2>
            <div class="tech-grid">
                <div class="tech-category">
                    <div class="category-title">Languages</div>
                    <div class="skills-list">
                        <span class="skill-tag">Java</span>
                        <span class="skill-tag">Kotlin</span>
                        <span class="skill-tag">Python</span>
                        <span class="skill-tag">JavaScript</span>
                    </div>
                </div>
                
                <div class="tech-category">
                    <div class="category-title">Android Development</div>
                    <div class="skills-list">
                        <span class="skill-tag">Room Database</span>
                        <span class="skill-tag">MVVM Architecture</span>
                        <span class="skill-tag">Jetpack Components</span>
                        <span class="skill-tag">LiveData</span>
                        <span class="skill-tag">ViewModel</span>
                        <span class="skill-tag">Navigation</span>
                    </div>
                </div>
                
                <div class="tech-category">
                    <div class="category-title">Other Skills</div>
                    <div class="skills-list">
                        <span class="skill-tag">API Integration</span>
                        <span class="skill-tag">UI/UX Design</span>
                        <span class="skill-tag">Debugging</span>
                        <span class="skill-tag">Optimization</span>
                    </div>
                </div>
            </div>
        </div>

        <div class="section">
            <h2 class="section-title">
                <span class="emoji">📈</span> GitHub Stats
            </h2>
            <div class="stats-placeholder">
                <p><strong>GitHub stats will be displayed here</strong></p>
                <p>You can add your GitHub stats images or widgets in this section</p>
            </div>
        </div>

        <div class="section">
            <h2 class="section-title">
                <span class="emoji">📫</span> Connect with Me
            </h2>
            <div class="contact-grid">
                <a href="https://www.linkedin.com/in/shantanu-pundir9/" class="contact-item" target="_blank">
                    <div class="contact-icon">💼</div>
                    <div>
                        <div>LinkedIn</div>
                        <div style="font-size: 0.9rem; opacity: 0.9;">Professional Network</div>
                    </div>
                </a>
                
                <a href="mailto:ranaaryan997@gmail.com" class="contact-item">
                    <div class="contact-icon">📧</div>
                    <div>
                        <div>Email</div>
                        <div style="font-size: 0.9rem; opacity: 0.9;">ranaaryan997@gmail.com</div>
                    </div>
                </a>
            </div>
        </div>
    </div>

    <script>
        // Create floating particles
        function createParticles() {
            const particlesContainer = document.querySelector('.particles');
            const particleCount = 50;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                
                // Random position
                particle.style.left = Math.random() * 100 + '%';
                particle.style.top = Math.random() * 100 + '%';
                
                // Random animation delay
                particle.style.animationDelay = Math.random() * 6 + 's';
                
                // Random animation duration
                particle.style.animationDuration = (Math.random() * 3 + 4) + 's';
                
                particlesContainer.appendChild(particle);
            }
        }

        // Skill tag click animation
        function addSkillInteractions() {
            const skillTags = document.querySelectorAll('.skill-tag');
            
            skillTags.forEach(tag => {
                tag.addEventListener('click', function() {
                    this.style.animation = 'none';
                    setTimeout(() => {
                        this.style.animation = 'bounce 0.5s ease';
                    }, 10);
                    
                    setTimeout(() => {
                        this.style.animation = '';
                    }, 500);
                });
            });
        }

        // Intersection Observer for animations
        function addScrollAnimations() {
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateX(0)';
                    }
                });
            }, { threshold: 0.1 });

            document.querySelectorAll('.section').forEach(section => {
                observer.observe(section);
            });
        }

        // Initialize everything when page loads
        document.addEventListener('DOMContentLoaded', function() {
            createParticles();
            addSkillInteractions();
            addScrollAnimations();
            
            // Add typing effect to name
            const nameElement = document.querySelector('.profile-name');
            const originalText = nameElement.textContent;
            nameElement.innerHTML = '<span class="emoji wave">👋</span> Hi, I\'m ';
            
            const nameSpan = document.createElement('span');
            nameElement.appendChild(nameSpan);
            
            let i = 0;
            const nameText = 'Shantanu Pundir';
            
            function typeWriter() {
                if (i < nameText.length) {
                    nameSpan.textContent += nameText.charAt(i);
                    i++;
                    setTimeout(typeWriter, 100);
                }
            }
            
            setTimeout(typeWriter, 500);
        });

        // Add parallax effect to container
        document.addEventListener('mousemove', function(e) {
            const container = document.querySelector('.container');
            const x = e.clientX / window.innerWidth;
            const y = e.clientY / window.innerHeight;
            
            container.style.transform = `translate(${x * 10 - 5}px, ${y * 10 - 5}px)`;
        });
    </script>
</body>
</html>
