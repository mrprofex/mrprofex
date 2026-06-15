<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>VIVEK KUMAR PATAR · Next Level GitHub Profile</title>
    <!-- Premium Fonts & Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,600;14..32,700;14..32,800&family=Space+Grotesk:wght@400;500;600;700&family=Orbitron:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- AOS Library for scroll animations -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0a0a0a;
            font-family: 'Inter', 'Space Grotesk', sans-serif;
            color: #f0f0f0;
            line-height: 1.5;
            scroll-behavior: smooth;
            overflow-x: hidden;
        }

        /* premium glassmorphism + neon glow */
        .glass-card {
            background: rgba(10, 10, 10, 0.65);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 106, 0, 0.3);
            border-radius: 2rem;
            box-shadow: 0 20px 35px -12px rgba(0,0,0,0.5), 0 0 0 1px rgba(255, 106, 0, 0.1) inset;
            transition: all 0.3s ease;
        }

        .glass-card:hover {
            border-color: rgba(255, 106, 0, 0.7);
            box-shadow: 0 25px 40px -12px rgba(255, 106, 0, 0.25), 0 0 0 1px rgba(255, 106, 0, 0.4) inset;
        }

        /* animated gradient text */
        .gradient-text {
            background: linear-gradient(135deg, #ff3c00, #ffaa33, #ff6a00, #ff3c00);
            background-size: 300% 300%;
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            animation: fireGradient 5s ease infinite;
            font-weight: 800;
        }

        @keyframes fireGradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* floating animation */
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-8px); }
            100% { transform: translateY(0px); }
        }

        .float-animation {
            animation: float 4s ease-in-out infinite;
        }

        /* typing cursor enhance */
        .cursor-blink {
            animation: blink 1s step-end infinite;
        }

        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }

        /* live pulse ring */
        .live-pulse {
            display: inline-block;
            width: 12px;
            height: 12px;
            background-color: #ff3c00;
            border-radius: 50%;
            box-shadow: 0 0 0 0 rgba(255, 60, 0, 0.7);
            animation: pulse-ring 1.5s infinite;
            margin-right: 8px;
        }

        @keyframes pulse-ring {
            0% { box-shadow: 0 0 0 0 rgba(255, 60, 0, 0.7); }
            70% { box-shadow: 0 0 0 8px rgba(255, 60, 0, 0); }
            100% { box-shadow: 0 0 0 0 rgba(255, 60, 0, 0); }
        }

        /* custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #111;
        }
        ::-webkit-scrollbar-thumb {
            background: #ff6a00;
            border-radius: 10px;
        }

        /* responsive container */
        .readme-container {
            max-width: 1300px;
            margin: 0 auto;
            padding: 2rem 1.5rem;
        }

        h1, h2, h3 {
            font-family: 'Orbitron', monospace;
            letter-spacing: -0.02em;
        }

        .tech-badge {
            transition: transform 0.2s ease, filter 0.2s;
        }
        .tech-badge:hover {
            transform: scale(1.08);
            filter: drop-shadow(0 0 12px #ff6a00);
        }

        /* snake container enhanced */
        .snake-wrapper {
            border-radius: 2rem;
            overflow: hidden;
            background: #00000022;
            backdrop-filter: blur(4px);
            border: 1px solid rgba(255,106,0,0.3);
        }

        /* responsive tables */
        @media (max-width: 780px) {
            .readme-container {
                padding: 1rem;
            }
            .glass-card {
                border-radius: 1.5rem;
            }
        }
    </style>
</head>
<body>

<div class="readme-container">

    <!-- ========== PREMIUM FIRE HEADER (capsule render style with extra layer) ========= -->
    <div data-aos="fade-down" data-aos-duration="1000">
        <div style="position: relative; border-radius: 2rem; overflow: hidden; margin-bottom: 2rem;">
            <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=340&text=VIVEK%20KUMAR%20PATAR&fontSize=52&fontColor=ffffff&animation=twinkling&fontAlignY=38&color=0:ff3c00,50:ff6a00,100:ff0000" alt="fire header" style="display: block;">
            <div style="position: absolute; bottom: 20px; left: 0; right: 0; text-align: center; font-size: 1.2rem; font-weight: 500; background: rgba(0,0,0,0.4); backdrop-filter: blur(5px); width: fit-content; margin: 0 auto; padding: 6px 24px; border-radius: 60px;">
                <span class="live-pulse"></span> LIVE CODING AURA
            </div>
        </div>
    </div>

    <!-- main greeting + typing SVG but enhanced with local JS for extra effect -->
    <div align="center" data-aos="zoom-in" data-aos-duration="800">
        <div style="background: rgba(0,0,0,0.3); border-radius: 3rem; padding: 1rem 0.5rem;">
            <div id="dynamic-typing" style="font-family: 'Orbitron', monospace; font-size: clamp(1.4rem, 5vw, 2.3rem); font-weight: 700; color: #ffaa33; letter-spacing: 1px;"></div>
        </div>
        <br>
        <img src="https://komarev.com/ghpvc/?username=mrprofex&label=🔥+PREMIUM+VIEWS&color=ff5500&style=for-the-badge" />
    </div>

    <!-- Developer Dashboard - 3D interactive cards -->
    <div class="dashboard-grid" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.8rem; margin: 3rem 0;" data-aos="fade-up" data-aos-delay="150">
        <div class="glass-card" style="padding: 1.5rem; text-align: center;">
            <i class="fas fa-terminal" style="font-size: 2.5rem; color: #ff6a00;"></i>
            <h3 style="margin-top: 0.8rem;">💻 VS CODE STATUS</h3>
            <div style="margin-top: 1rem;">
                <p><span class="live-pulse"></span> <strong style="color:#ffaa33;">Active Coding Mode</strong></p>
                <p>🔥 Building Projects</p>
                <p>⚡ Debugging Skills</p>
                <p>🚀 Learning Every Day</p>
            </div>
            <div class="progress-bar" style="height: 4px; background: #222; border-radius: 4px; margin-top: 1rem;"><div style="width: 94%; background: #ff6a00; height: 4px; border-radius: 4px;"></div></div>
        </div>
        <div class="glass-card" style="padding: 1.5rem; text-align: center;">
            <i class="fas fa-rocket" style="font-size: 2.5rem; color: #ff6a00;"></i>
            <h3 style="margin-top: 0.8rem;">🎯 MISSION STATUS</h3>
            <p>🚀 Full Stack Goal</p>
            <p>🔥 Daily Practice</p>
            <p>⚡ Project Building</p>
            <p>💡 Growth Mode</p>
            <div style="margin-top: 12px;"><span class="badge" style="background: #ff6a0022; border: 1px solid #ff6a00; border-radius: 60px; padding: 4px 12px;">ACTIVE · 100%</span></div>
        </div>
        <div class="glass-card" style="padding: 1.5rem; text-align: center;">
            <i class="fas fa-satellite-dish" style="font-size: 2.5rem; color: #ff6a00;"></i>
            <h3 style="margin-top: 0.8rem;">📡 LIVE SYSTEM</h3>
            <p><span class="live-pulse"></span> <strong>Online</strong></p>
            <p>⚙️ Processing Skills</p>
            <p>📈 Improving Daily</p>
            <p>💾 Saving Knowledge</p>
        </div>
    </div>

    <!-- Connect Section with hover animations -->
    <div align="center" data-aos="flip-up" data-aos-duration="700">
        <h2 class="gradient-text" style="font-size: 2rem;"><i class="fas fa-plug"></i> CONNECT & COLLABORATE</h2>
        <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 1rem; margin: 1.5rem 0;">
            <a href="https://instagram.com/vivek.kr.patar" target="_blank"><img src="https://img.shields.io/badge/Instagram-FF5500?style=for-the-badge&logo=instagram&logoColor=white" class="tech-badge"/></a>
            <a href="https://linkedin.com/in/vivek-kumar-patar-064953369" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-ff6600?style=for-the-badge&logo=linkedin&logoColor=white" class="tech-badge"/></a>
            <a href="https://github.com/mrprofex" target="_blank"><img src="https://img.shields.io/badge/GitHub-111111?style=for-the-badge&logo=github&logoColor=white" class="tech-badge"/></a>
            <a href="https://wa.me/917970586436" target="_blank"><img src="https://img.shields.io/badge/WhatsApp-ff3300?style=for-the-badge&logo=whatsapp&logoColor=white" class="tech-badge"/></a>
        </div>
    </div>

    <!-- SYSTEM ONLINE BANNER -->
    <div align="center" style="margin: 2rem 0;" data-aos="zoom-in">
        <img width="100%" src="https://capsule-render.vercel.app/api?type=rect&height=120&text=⟁%20SYSTEM%20ONLINE%20⟁&fontColor=00ff88&fontSize=38&animation=blinking&color=0:000000,100:001100" />
    </div>

    <!-- Journey & Tech Stack together with glassmorphism -->
    <div style="display: flex; flex-wrap: wrap; gap: 2rem; margin: 2rem 0;">
        <div class="glass-card" style="flex:1; padding: 1.6rem;" data-aos="fade-right">
            <h2><i class="fas fa-globe-asia"></i> 🌍 CURRENT JOURNEY</h2>
            <ul style="margin-top: 1rem; list-style: none;">
                <li>🧠 <strong>Modern Web Dev</strong> - Mastery path</li>
                <li>⚡ <strong>Responsive & Animations</strong></li>
                <li>🎯 <strong>Problem Solving</strong> - DSA grind</li>
                <li>🚀 <strong>AI & future tech</strong> exploration</li>
                <li>🔥 <strong>Consistent shipping</strong> projects</li>
            </ul>
        </div>
        <div class="glass-card" style="flex:1; padding: 1.6rem;" data-aos="fade-left">
            <h2><i class="fas fa-cogs"></i> 🛠 TECH STACK (EXPERTISE)</h2>
            <div align="center" style="margin-top: 1rem;">
                <img src="https://skillicons.dev/icons?i=vscode,python,java,html,css,js,react,nodejs,git,github,tailwind,figma" style="max-width:100%;" class="tech-badge"/>
            </div>
            <p align="center" style="margin-top: 1rem;"><span class="gradient-text">#FullStackReady</span></p>
        </div>
    </div>

    <!-- ADVANCED GITHUB STATS + ACTIVITY GRAPH + CARDS WITH INTERACTIVE -->
    <div data-aos="fade-up">
        <h2 align="center" class="gradient-text"><i class="fas fa-chart-line"></i> ⚡ DEVELOPER ACTIVITY MATRIX</h2>
        <div style="display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center; margin: 2rem 0;">
            <div class="glass-card" style="padding: 1rem; background: #0b0b0b;"><img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=mrprofex&theme=github_dark" width="100%"/></div>
            <div class="glass-card" style="padding: 1rem;"><img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=mrprofex&theme=github_dark&utcOffset=8" width="100%"/></div>
            <div class="glass-card" style="padding: 1rem; grid-column: span 2;"><img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=mrprofex&theme=github_dark" width="100%"/></div>
        </div>
        <div class="glass-card" style="padding: 1rem; overflow: hidden;">
            <img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=mrprofex&theme=tokyo-night&hide_border=true&area=true&bg_color=000000&color=ff6a00&line=ff6a00&point=ffffff" alt="activity graph"/>
        </div>
    </div>

    <!-- STREAK + ACHIEVEMENTS modern row -->
    <div style="display: flex; flex-wrap: wrap; gap: 2rem; margin: 2.5rem 0;" data-aos="fade-up">
        <div class="glass-card" style="flex: 1.5; padding: 1rem;">
            <img src="https://streak-stats.demolab.com/?user=mrprofex&theme=tokyonight&hide_border=true&stroke=ff6a00&ring=ff6a00&fire=ff6a00&currStreakNum=ffffff&sideNums=ffffff&currStreakLabel=ff6a00&sideLabels=ffffff&dates=ffffff" width="100%" alt="streak"/>
        </div>
        <div class="glass-card" style="flex: 1; padding: 1.5rem;">
            <h3 align="center"><i class="fas fa-trophy"></i> 🏆 ACHIEVEMENTS</h3>
            <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 8px; margin-top: 1rem;">
                <span>🏅 Consistent Learner</span><span>🏅 Frontend Mastery</span>
                <span>🏅 Open Source Journey</span><span>🏅 Weekly Builder</span>
                <span>🏅 AI Explorer</span><span>🏅 200+ Commits</span>
            </div>
        </div>
    </div>

    <!-- FEATURED PROJECTS + DYNAMIC INSIGHT -->
    <div style="background: linear-gradient(145deg, #0f0f0f, #050505); border-radius: 2rem; padding: 1.8rem; margin: 2rem 0; border-left: 5px solid #ff6a00;" data-aos="flip-left">
        <h2 align="center" style="font-size: 2rem;"><i class="fas fa-crown"></i> 🚀 NEXT-GEN PROJECTS</h2>
        <div style="display: flex; flex-wrap: wrap; justify-content: space-between; gap: 1rem;">
            <div><i class="fas fa-globe"></i> <strong>🌐 Portfolio 360°</strong><br>Immersive 3D experience</div>
            <div><i class="fas fa-tasks"></i> <strong>📝 Hyper To-Do</strong><br>AI-powered task management</div>
            <div><i class="fas fa-calculator"></i> <strong>🧮 Quantum Calc</strong><br>NextJS + animations</div>
            <div><i class="fas fa-brain"></i> <strong>🤖 AI Chat Interface</strong><br>GPT integration incoming</div>
        </div>
    </div>

    <!-- SPOTLIGHT + LIVE CODING SESSION WITH DEVELOPER SPOTLIGHT GIF -->
    <div align="center" data-aos="fade-up">
        <div class="glass-card" style="padding: 1.5rem;">
            <img width="100%" src="https://user-images.githubusercontent.com/74038190/221352995-5ac18bdf-1a19-4f99-bbb6-77559b220470.gif" style="border-radius: 1rem;">
            <div id="liveCounter" style="margin: 1rem 0; font-family: monospace; font-size: 1.4rem; color: #ffaa33;">
                🎥 LIVE SESSION: <span id="sessionTimer">00:00:00</span> • coding flow active
            </div>
            <table style="width: 100%; margin-top: 10px;">
                <tr><td>🎯 TODAY'S FOCUS</td><td>🚀 PROJECT</td><td>⏰ SESSION TIME</td></tr>
                <tr><td><strong>Full Stack Dev + AI</strong></td><td><strong>Portfolio 3.0</strong></td><td><strong id="liveHours">6h 42m</strong></td></tr>
            </table>
        </div>
    </div>

    <!-- Dev Tunes - Spotify style with interactive pulse -->
    <div align="center" data-aos="zoom-in-up">
        <h2><i class="fas fa-headphones"></i> 🎧 DEV BEATS (CODING VIBES)</h2>
        <div style="display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap; margin: 1rem 0;">
            <a href="https://open.spotify.com/playlist/37i9dQZF1DX3Ogo9pFvBkY" target="_blank"><img src="https://img.shields.io/badge/CODING%20PLAYLIST-Lofi%20Beats-ff6a00?style=for-the-badge&logo=spotify"/></a>
            <a href="https://music.youtube.com/playlist?list=RDCLAK5uy_kmrX0Vl4z0ui6vNnF9g7Az7gGZb_5Jvq8" target="_blank"><img src="https://img.shields.io/badge/FOCUS%20MIX-Chill%20Vibes-ff8800?style=for-the-badge"/></a>
        </div>
        <div class="glass-card" style="display: inline-block; padding: 0.5rem 1.5rem;">🎵 *click badge → instant coding soundtrack* 🎵</div>
    </div>

    <!-- INTERACTIVE STATS DASHBOARD (extra next level) -->
    <div align="center" style="margin: 2rem 0;" data-aos="fade-right">
        <img width="100%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=mrprofex&theme=gruvbox" class="glass-card" style="border-radius: 2rem;">
    </div>

    <!-- Mermaid Learning Roadmap animated with shiny effect -->
    <div class="glass-card" style="padding: 1.8rem; margin: 2rem 0;" data-aos="fade-up">
        <h2 align="center">🗺️ ADVANCED LEARNING ROADMAP</h2>
        <pre style="background: #00000055; color:#ffcc88; border-radius: 1rem; padding: 1rem; overflow-x: auto; font-size: 0.8rem;">
[HTML/CSS] → [JS ES6+] → [React+Redux] → [Node+Express] → [MongoDB] → [Full Stack Apps]
                     ↘ [TypeScript] → [Next.js] → [Performance & AI integration]
        </pre>
        <div align="center"><span class="gradient-text">⚡ Currently: Full Stack mastery + AI explorations ⚡</span></div>
    </div>

    <!-- FUN FACTS + SNAKE ANIMATION reimagined with glow -->
    <div style="display: flex; flex-wrap: wrap; gap: 1.5rem; margin-top: 2rem;">
        <div class="glass-card" style="flex: 1; padding: 1.5rem;" data-aos="fade-right">
            <h3>☕ FUN FACTS</h3>
            <p>💻 I code with 🔥 intensity and midnight oil</p>
            <p>🌙 Late-night builds bring magic</p>
            <p>🎯 Turning coffee → code → impact</p>
            <p>✨ Believer of open source and creative experiments</p>
        </div>
        <div class="glass-card" style="flex: 2; padding: 1rem;" data-aos="fade-left">
            <div class="snake-wrapper">
                <img width="100%" src="https://raw.githubusercontent.com/Platane/snk/output/github-contribution-grid-snake-dark.svg" alt="snake animation"/>
            </div>
        </div>
    </div>

    <!-- FOOTER : NEXT LEVEL ALERT -->
    <div align="center" style="margin: 3rem 0 1rem;" data-aos="flip-up">
        <img src="https://readme-typing-svg.herokuapp.com?font=Orbitron&weight=800&size=24&duration=1400&pause=300&color=FF4500&center=true&vCenter=true&width=900&lines=🔥+NEXT+LEVEL+DEVELOPER+MINDSET;✨+VIVEK+KUMAR+PATAR+•+BUILDING+TOMORROW;⚡+COMMIT+•+CREATE+•+REPEAT" />
        <br><br>
        <div style="font-size: 0.8rem; opacity: 0.7;">© 2026 VIVEK KUMAR PATAR — full throttle dev experience</div>
    </div>
</div>

<!-- JavaScript: dynamic typing effect + live session timer (next level interactivity) -->
<script>
    // premium dynamic typing (simulating real-time system)
    const phrases = [
        "🔥 CODE · CREATE · REPEAT",
        "💻 COMPUTER SCIENCE ENGINEER",
        "🚀 FRONTEND + AI EXPLORER",
        "⚡ BUILDING PROJECTS EVERY DAY",
        "🌟 VIVEK KUMAR PATAR · NEXT LEVEL"
    ];
    let idx = 0;
    let charIndex = 0;
    let currentText = "";
    let isDeleting = false;
    const typingElement = document.getElementById("dynamic-typing");
    function typeEffect() {
        const fullText = phrases[idx];
        if (isDeleting) {
            currentText = fullText.substring(0, charIndex - 1);
            charIndex--;
        } else {
            currentText = fullText.substring(0, charIndex + 1);
            charIndex++;
        }
        typingElement.innerHTML = currentText + '<span class="cursor-blink" style="color:#ff6a00;">|</span>';
        if (!isDeleting && charIndex === fullText.length) {
            isDeleting = true;
            setTimeout(typeEffect, 1800);
        } else if (isDeleting && charIndex === 0) {
            isDeleting = false;
            idx = (idx + 1) % phrases.length;
            setTimeout(typeEffect, 300);
        } else {
            let speed = isDeleting ? 50 : 100;
            setTimeout(typeEffect, speed);
        }
    }
    typeEffect();

    // Live Session Timer (next-level immersive)
    let startTime = new Date();
    startTime.setHours(6, 42, 0);  // starting from 6h 42m as inspiration
    let secondsElapsed = (6 * 3600) + (42 * 60);
    const timerElement = document.getElementById("sessionTimer");
    const liveHoursSpan = document.getElementById("liveHours");

    function updateTimer() {
        secondsElapsed++;
        const hrs = Math.floor(secondsElapsed / 3600);
        const mins = Math.floor((secondsElapsed % 3600) / 60);
        const secs = secondsElapsed % 60;
        timerElement.innerText = `${hrs.toString().padStart(2,'0')}:${mins.toString().padStart(2,'0')}:${secs.toString().padStart(2,'0')}`;
        liveHoursSpan.innerText = `${hrs}h ${mins}m`;
    }
    setInterval(updateTimer, 1000);
</script>
<!-- AOS initialization -->
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
<script>
    AOS.init({
        duration: 900,
        once: false,
        mirror: true,
    });
    // additional glitch effect for fancy display
    console.log("%c🔥 VIVEK KUMAR PATAR | NEXT LEVEL READY", "color: #ff6a00; font-size: 18px; font-weight: bold;");
</script>
</body>
</html>
