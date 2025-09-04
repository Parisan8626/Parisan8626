<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Parisan8626 - GitHub Profile</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0d1117 0%, #161b22 100%);
            color: #c9d1d9;
            line-height: 1.6;
            padding: 20px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
            margin-bottom: 30px;
            background: rgba(13, 17, 23, 0.8);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            border: 1px solid #30363d;
        }
        
        .profile-info {
            display: flex;
            align-items: center;
            gap: 20px;
        }
        
        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 4px solid #58a6ff;
            object-fit: cover;
        }
        
        .profile-text h1 {
            font-size: 28px;
            color: #58a6ff;
            margin-bottom: 5px;
        }
        
        .profile-text p {
            color: #8b949e;
            font-size: 18px;
        }
        
        .stats {
            display: flex;
            gap: 20px;
            background: rgba(22, 27, 34, 0.8);
            padding: 15px;
            border-radius: 10px;
            border: 1px solid #30363d;
        }
        
        .stat-item {
            text-align: center;
        }
        
        .stat-number {
            font-size: 24px;
            font-weight: bold;
            color: #58a6ff;
        }
        
        .stat-label {
            font-size: 14px;
            color: #8b949e;
        }
        
        .section {
            background: rgba(13, 17, 23, 0.8);
            margin-bottom: 30px;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            border: 1px solid #30363d;
        }
        
        .section-title {
            color: #58a6ff;
            font-size: 24px;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid #30363d;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .skill-category {
            background: rgba(22, 27, 34, 0.8);
            padding: 20px;
            border-radius: 10px;
            border: 1px solid #30363d;
        }
        
        .skill-category h3 {
            color: #58a6ff;
            margin-bottom: 15px;
            font-size: 18px;
        }
        
        .skill-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .skill {
            background: rgba(56, 139, 253, 0.15);
            color: #58a6ff;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 14px;
            border: 1px solid rgba(56, 139, 253, 0.4);
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .project-card {
            background: rgba(22, 27, 34, 0.8);
            border-radius: 10px;
            overflow: hidden;
            border: 1px solid #30363d;
            transition: transform 0.3s ease;
        }
        
        .project-card:hover {
            transform: translateY(-5px);
        }
        
        .project-content {
            padding: 20px;
        }
        
        .project-title {
            color: #58a6ff;
            font-size: 18px;
            margin-bottom: 10px;
        }
        
        .project-desc {
            color: #8b949e;
            font-size: 14px;
            margin-bottom: 15px;
        }
        
        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 15px;
        }
        
        .tech-tag {
            background: rgba(56, 139, 253, 0.15);
            color: #58a6ff;
            padding: 3px 10px;
            border-radius: 15px;
            font-size: 12px;
            border: 1px solid rgba(56, 139, 253, 0.4);
        }
        
        .contribution-graph {
            background: rgba(22, 27, 34, 0.8);
            padding: 20px;
            border-radius: 10px;
            border: 1px solid #30363d;
            margin-bottom: 20px;
        }
        
        .graph-placeholder {
            height: 150px;
            background: linear-gradient(90deg, #0d1117 0%, #161b22 100%);
            border-radius: 5px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #8b949e;
            font-size: 16px;
        }
        
        .graph-key {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 15px;
        }
        
        .graph-key-item {
            display: flex;
            align-items: center;
            gap: 5px;
            font-size: 12px;
            color: #8b949e;
        }
        
        .key-color {
            width: 12px;
            height: 12px;
            border-radius: 2px;
        }
        
        .contribution-stats {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 15px;
        }
        
        .contribution-stat {
            background: rgba(22, 27, 34, 0.8);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            border: 1px solid #30363d;
        }
        
        .contribution-stat .number {
            font-size: 24px;
            font-weight: bold;
            color: #58a6ff;
            margin-bottom: 5px;
        }
        
        .contribution-stat .label {
            font-size: 14px;
            color: #8b949e;
        }
        
        .gif-container {
            text-align: center;
            padding: 20px;
            background: rgba(22, 27, 34, 0.8);
            border-radius: 10px;
            border: 1px solid #30363d;
        }
        
        .stars-gif {
            width: 200px;
            height: 200px;
            background: linear-gradient(45deg, #0d1117, #161b22, #0d1117);
            border-radius: 50%;
            margin: 0 auto;
            position: relative;
            overflow: hidden;
        }
        
        .star {
            position: absolute;
            background-color: #58a6ff;
            border-radius: 50%;
            animation: twinkle 2s infinite;
        }
        
        @keyframes twinkle {
            0% { opacity: 0.2; }
            50% { opacity: 1; }
            100% { opacity: 0.2; }
        }
        
        footer {
            text-align: center;
            margin-top: 40px;
            padding: 20px;
            color: #8b949e;
            font-size: 14px;
            border-top: 1px solid #30363d;
        }
        
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                text-align: center;
                gap: 20px;
            }
            
            .profile-info {
                flex-direction: column;
            }
            
            .stats {
                justify-content: center;
            }
            
            .skills-container, .projects-grid, .contribution-stats {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="profile-info">
                <img class="avatar" src="https://avatars.githubusercontent.com/u/133004133?v=4" alt="Profile Avatar">
                <div class="profile-text">
                    <h1>Parisan8626</h1>
                    <p>Frontend Developer & ML Enthusiast</p>
                </div>
            </div>
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number">12</div>
                    <div class="stat-label">Repositories</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">284</div>
                    <div class="stat-label">Contributions</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">8</div>
                    <div class="stat-label">Projects</div>
                </div>
            </div>
        </header>
        
        <section class="section">
            <h2 class="section-title"><i class="fas fa-user"></i> About Me</h2>
            <p>Frontend developer with experience in Python and Machine Learning. Skilled in creating responsive and user-friendly web applications using modern technologies.</p>
        </section>
        
        <section class="section">
            <h2 class="section-title"><i class="fas fa-code"></i> Skills & Technologies</h2>
            <div class="skills-container">
                <div class="skill-category">
                    <h3>Frontend</h3>
                    <div class="skill-list">
                        <span class="skill">HTML</span>
                        <span class="skill">CSS</span>
                        <span class="skill">JavaScript</span>
                        <span class="skill">React</span>
                        <span class="skill">Next.js</span>
                        <span class="skill">Tailwind CSS</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>Development Tools</h3>
                    <div class="skill-list">
                        <span class="skill">Git</span>
                        <span class="skill">GitHub</span>
                        <span class="skill">VS Code</span>
                        <span class="skill">Figma</span>
                        <span class="skill">Vite</span>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>Other</h3>
                    <div class="skill-list">
                        <span class="skill">Python</span>
                        <span class="skill">Machine Learning</span>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="section">
            <h2 class="section-title"><i class="fas fa-project-diagram"></i> Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <div class="project-content">
                        <h3 class="project-title">Traffic Light</h3>
                        <p class="project-desc">A simulation of traffic lights with interactive controls.</p>
                        <div class="project-tech">
                            <span class="tech-tag">HTML</span>
                            <span class="tech-tag">CSS</span>
                            <span class="tech-tag">JavaScript</span>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-content">
                        <h3 class="project-title">Tic Tac Toe</h3>
                        <p class="project-desc">Interactive Tic Tac Toe game with win detection.</p>
                        <div class="project-tech">
                            <span class="tech-tag">React</span>
                            <span class="tech-tag">Tailwind CSS</span>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-content">
                        <h3 class="project-title">Weather App</h3>
                        <p class="project-desc">Real-time weather information application.</p>
                        <div class="project-tech">
                            <span class="tech-tag">Next.js</span>
                            <span class="tech-tag">API</span>
                        </div>
                    </div>
                </div>
                
                <div class="project-card">
                    <div class="project-content">
                        <h3 class="project-title">Pet Grooming Website</h3>
                        <p class="project-desc">Two-page website for a pet grooming salon.</p>
                        <div class="project-tech">
                            <span class="tech-tag">Figma</span>
                            <span class="tech-tag">HTML</span>
                            <span class="tech-tag">CSS</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="section">
            <h2 class="section-title"><i class="fas fa-chart-line"></i> Contribution Metrics</h2>
            <div class="contribution-graph">
                <div class="graph-placeholder">
                    Contribution Graph Visualization
                </div>
                <div class="graph-key">
                    <div class="graph-key-item">
                        <div class="key-color" style="background-color: #ebedf0"></div>
                        <span>Less</span>
                    </div>
                    <div class="graph-key-item">
                        <div class="key-color" style="background-color: #9be9a8"></div>
                        <span>More</span>
                    </div>
                </div>
            </div>
            
            <div class="contribution-stats">
                <div class="contribution-stat">
                    <div class="number">284</div>
                    <div class="label">Total Contributions</div>
                </div>
                <div class="contribution-stat">
                    <div class="number">42</div>
                    <div class="label">Longest Streak</div>
                </div>
                <div class="contribution-stat">
                    <div class="number">12</div>
                    <div class="label">Current Streak</div>
                </div>
            </div>
        </section>
        
        <section class="section">
            <h2 class="section-title"><i class="fas fa-star"></i> Animated Stars</h2>
            <div class="gif-container">
                <div class="stars-gif" id="starsGif"></div>
                <p style="margin-top: 15px;">Blue twinkling stars animation</p>
            </div>
        </section>
        
        <footer>
            <p>GitHub Profile • Parisan8626 • 2023</p>
        </footer>
    </div>

    <script>
        // Create animated stars
        function createStars() {
            const container = document.getElementById('starsGif');
            const starsCount = 50;
            
            for (let i = 0; i < starsCount; i++) {
                const star = document.createElement('div');
                star.classList.add('star');
                
                // Random size between 2px and 6px
                const size = Math.random() * 4 + 2;
                star.style.width = `${size}px`;
                star.style.height = `${size}px`;
                
                // Random position
                const x = Math.random() * 100;
                const y = Math.random() * 100;
                star.style.left = `${x}%`;
                star.style.top = `${y}%`;
                
                // Random animation delay
                const delay = Math.random() * 5;
                star.style.animationDelay = `${delay}s`;
                
                container.appendChild(star);
            }
        }
        
        // Initialize when page loads
        window.onload = function() {
            createStars();
        };
    </script>
</body>
</html>
