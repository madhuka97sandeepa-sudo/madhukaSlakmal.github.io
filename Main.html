<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Madhuka | VFX & 3D Artist</title>
    
    <!-- Fonts: Orbitron for sci-fi headers, Rajdhani for technical text -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Rajdhani:wght@300;500;700&display=swap" rel="stylesheet">

    <style>
        :root {
            --bg-deep: #050508;
            --accent: #00f3ff; /* Neon Cyan */
            --accent-dim: rgba(0, 243, 255, 0.2);
            --secondary: #ff0055; /* Neon Pink/Red for errors/alerts or secondary pop */
            --text-main: #e0e0e0;
            --glass: rgba(10, 15, 30, 0.75);
            --border-glass: rgba(0, 243, 255, 0.3);
            --font-head: 'Orbitron', sans-serif;
            --font-body: 'Rajdhani', sans-serif;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            background-color: var(--bg-deep);
            color: var(--text-main);
            font-family: var(--font-body);
            overflow-x: hidden;
            /* Enable 3D perspective on the whole body */
            perspective: 1000px; 
        }

        /* --- STAR FIELD BACKGROUND (Simulating 3D Space) --- */
        .stars {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            z-index: -1;
            background: 
                radial-gradient(white, rgba(255,255,255,.2) 2px, transparent 3px),
                radial-gradient(white, rgba(255,255,255,.15) 1px, transparent 2px),
                radial-gradient(white, rgba(255,255,255,.1) 2px, transparent 3px);
            background-size: 550px 550px, 350px 350px, 250px 250px;
            background-position: 0 0, 40px 60px, 130px 270px;
            animation: starMove 100s linear infinite;
        }
        
        @keyframes starMove { from { transform: translateY(0); } to { transform: translateY(-1000px); } }

        /* --- 3D PLACEHOLDER STYLES --- */
        /* These styles represent where your OBJ models will go */
        .model-stage {
            width: 100%;
            height: 400px;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 1px dashed var(--accent-dim);
            background: radial-gradient(circle, rgba(0,243,255,0.05) 0%, transparent 70%);
        }

        .placeholder-box {
            width: 150px;
            height: 150px;
            border: 2px solid var(--accent);
            background: rgba(0, 243, 255, 0.1);
            position: absolute;
            transform-style: preserve-3d;
            animation: float 6s ease-in-out infinite;
        }
        
        /* A wireframe cube representation */
        .placeholder-box::before, .placeholder-box::after {
            content: ''; position: absolute; width: 100%; height: 100%; border: 1px solid var(--accent);
        }
        .placeholder-box::after { transform: translateZ(50px); }
        
        .label-3d {
            position: absolute; bottom: 10px; right: 10px;
            font-family: var(--font-head); font-size: 0.8rem; color: var(--accent);
            background: rgba(0,0,0,0.8); padding: 2px 8px;
        }

        @keyframes float { 
            0%, 100% { transform: translateY(0) rotateX(10deg) rotateY(10deg); } 
            50% { transform: translateY(-20px) rotateX(-10deg) rotateY(-10deg); } 
        }

        /* --- NAVIGATION & HOVER POPUPS --- */
        nav {
            position: fixed;
            top: 0; left: 0; width: 100%;
            padding: 0 2rem;
            height: 80px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(5, 5, 8, 0.8);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid var(--border-glass);
            z-index: 1000;
        }

        .logo {
            font-family: var(--font-head);
            font-size: 1.5rem;
            color: var(--accent);
            text-shadow: 0 0 10px var(--accent);
        }

        .nav-container {
            display: flex;
            gap: 2rem;
            height: 100%;
            align-items: center;
        }

        .nav-item {
            position: relative;
            height: 80px; /* Full height for hover trigger */
            display: flex;
            align-items: center;
            cursor: pointer;
        }

        .nav-link {
            font-family: var(--font-head);
            font-size: 0.9rem;
            letter-spacing: 1px;
            color: #fff;
            padding: 0.5rem 1rem;
            transition: 0.3s;
            border: 1px solid transparent;
        }

        .nav-item:hover .nav-link {
            background: var(--accent-dim);
            border-color: var(--accent);
            box-shadow: 0 0 15px var(--accent-dim);
        }

        /* --- POPUP DATA PODS --- */
        .popup-content {
            position: absolute;
            top: 85px; /* Just below the nav bar */
            left: 50%;
            transform: translateX(-50%) translateY(20px);
            width: 350px;
            background: var(--glass);
            border: 1px solid var(--border-glass);
            border-radius: 8px;
            padding: 1.5rem;
            backdrop-filter: blur(15px);
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            
            /* Tech look */
            clip-path: polygon(10% 0, 100% 0, 100% 90%, 90% 100%, 0 100%, 0 10%);
        }

        /* Popup Arrow */
        .popup-content::before {
            content: '';
            position: absolute;
            top: -6px; left: 50%; transform: translateX(-50%);
            border-left: 6px solid transparent;
            border-right: 6px solid transparent;
            border-bottom: 6px solid var(--accent);
        }

        .nav-item:hover .popup-content {
            opacity: 1;
            visibility: visible;
            transform: translateX(-50%) translateY(0);
        }

        .popup-title {
            font-family: var(--font-head);
            color: var(--accent);
            font-size: 1.1rem;
            margin-bottom: 1rem;
            border-bottom: 1px solid rgba(255,255,255,0.1);
            padding-bottom: 0.5rem;
        }

        .popup-text {
            font-size: 0.95rem;
            line-height: 1.5;
            color: #ccc;
            white-space: pre-wrap; /* Preserves line breaks from your input */
        }
        
        .popup-text strong { color: #fff; }

        /* --- SECTIONS --- */
        section {
            padding: 120px 2rem 50px;
            min-height: 80vh;
            max-width: 1200px;
            margin: 0 auto;
            position: relative;
            transform-style: preserve-3d;
        }

        h2 {
            font-family: var(--font-head);
            font-size: 3rem;
            color: #fff;
            margin-bottom: 2rem;
            text-transform: uppercase;
        }

        .card-3d {
            background: linear-gradient(135deg, rgba(255,255,255,0.03), rgba(255,255,255,0.01));
            border: 1px solid rgba(255,255,255,0.1);
            padding: 2rem;
            margin-bottom: 2rem;
            transform: translateZ(0); /* Reset for hover */
            transition: transform 0.3s;
        }

        .card-3d:hover {
            transform: translateZ(30px) rotateX(2deg);
            border-color: var(--accent);
            box-shadow: 0 10px 40px rgba(0,0,0,0.5);
        }

        /* --- SPECIFIC POPUP OVERRIDES --- */
        /* Adjust width for specific items if needed */
        .nav-item#nav-about .popup-content { width: 400px; }
        .nav-item#nav-contact .popup-content { width: 350px; }

    </style>
</head>
<body>

    <div class="stars"></div>

    <!-- NAVIGATION BAR -->
    <nav>
        <div class="logo">MADHUKA.DESIGN</div>
        
        <div class="nav-container">
            
            <!-- ABOUT POPUP -->
            <div class="nav-item" id="nav-about">
                <span class="nav-link">ABOUT</span>
                <div class="popup-content">
                    <div class="popup-title">ABOUT ME</div>
                    <div class="popup-text">HELLO! I'M MADHUKA, A SEASONED VFX ARTIST WITH MORE THAN THREE YEARS OF EXPERIENCE. I SPECIALIZE IN CREATING REALISTIC 3D MODELS FOR GAMING, PRODUCTION, AND ANIMATION.

SKILLED IN: BLENDER, 3DS MAX, MAYA, HOUDINI, SUBSTANCE PAINTER, KEY SHOT, UNREAL ENGINE, AND UNITY. MY EXPERTISE INCLUDES A THOROUGH GRASP OF SECTION FLOWS, MATERIALS, AND COLORS, RESULTING IN VISUALLY ATTRACTIVE CONTENT. I ALSO HAVE EXPERIENCE COMPOSING IN AFTER EFFECTS, PREMIERE PRO, AND DAVINCI RESOLVE.

CLIENTS: MANTRA FILMS COLOMBO, IDEAL SEMICONDUCTOR (USA), CHEQD (UK), AND OTHERS.</div>
                </div>
            </div>

            <!-- EXPERIENCE POPUP -->
            <div class="nav-item" id="nav-experience">
                <span class="nav-link">EXPERIENCE</span>
                <div class="popup-content">
                    <div class="popup-title">CAREER TIMELINE</div>
                    <div class="popup-text">
<strong>SENIOR CREATIVE</strong> @ Rubiq Creatives (2024 - Present)<br>
<strong>CREATIVE</strong> @ Ada Global (Mar 2024 - July 2024)<br>
<strong>3D ARTIST</strong> @ Mantra Films (May 2023 - Sep 2023)<br>
<strong>GAME DESIGNER</strong> @ Heladev (Sep 2020 - Sep 2021)<br>
<strong>3D LECTURER</strong> @ Wijaya Graphic (Oct 2019 - Mar 2020)<br>
<strong>FREELANCER</strong> (Oct 2019 - Present)
                    </div>
                </div>
            </div>

            <!-- WORK POPUP -->
            <div class="nav-item" id="nav-work">
                <span class="nav-link">WORK</span>
                <div class="popup-content">
                    <div class="popup-title">SELECTED WORKS</div>
                    <div class="popup-text">
<strong>MUSIC VIDEOS:</strong> M-Tune Series (Mantra Films)<br>
<strong>ADVERTISING:</strong> Wireman Switch, Elephant House (Orange)<br>
<strong>GAMES:</strong> Panbatta, Snow Ball (Heladev)<br>
<strong>INTERNATIONAL:</strong> Ideal Semiconductor (USA), Cheqd (UK)<br>
<strong>COMMERCIALS:</strong> 0777, Studio of Dracary
                    </div>
                </div>
            </div>

            <!-- SKILLS POPUP -->
            <div class="nav-item" id="nav-skills">
                <span class="nav-link">SKILLS</span>
                <div class="popup-content">
                    <div class="popup-title">SOFTWARE SKILLS</div>
                    <div class="popup-text" style="display:flex; flex-wrap:wrap; gap:5px;">
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">BLENDER</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">3DS MAX</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">MAYA</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">HOUDINI</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">UNREAL ENGINE</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">UNITY</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">SUBSTANCE PAINTER</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">AFTER EFFECTS</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">PREMIERE PRO</span>
                        <span style="background:rgba(0,243,255,0.2); padding:2px 6px; border:1px solid var(--accent);">DAVINCI RESOLVE</span>
                    </div>
                </div>
            </div>

            <!-- CONTACT POPUP -->
            <div class="nav-item" id="nav-contact">
                <span class="nav-link">CONTACT</span>
                <div class="popup-content">
                    <div class="popup-title">CONTACT ME</div>
                    <div class="popup-text">
<strong>EMAIL:</strong><br>
<a href="mailto:MADHUKA97SANDEEPA@GMAIL.COM" style="color:var(--accent);">MADHUKA97SANDEEPA@GMAIL.COM</a><br><br>

<strong>PHONE:</strong><br>
+94 70 676 85 85<br><br>

<strong>ADDRESS:</strong><br>
POLWATHTHA RD, BATAMANDIYA,<br>
NIKAGODA, KALAWANA
                    </div>
                </div>
            </div>

        </div>
    </nav>

    <!-- HERO SECTION (Main 3D Stage) -->
    <section id="home">
        <h2 style="position: absolute; top: -40px; left: 0; font-size: 8rem; opacity: 0.1; pointer-events: none;">HELLO</h2>
        
        <!-- 3D PLACEHOLDER: Main Character / Model -->
        <div class="model-stage">
            <!-- TODO: Add Three.js canvas here or an iframe for your main OBJ/GLTF viewer -->
            <div class="placeholder-box"></div>
            <div class="label-3d">MAIN_SHOWCASE.OBJ</div>
        </div>

        <div class="card-3d" style="margin-top: -50px; position: relative; z-index: 2;">
            <h1>VFX & 3D ARTIST</h1>
            <p>Welcome to my digital workspace. Hover over the menu above to explore my data logs.</p>
        </div>
    </section>

    <!-- WORK PREVIEW SECTION (Floating Cards) -->
    <section id="work-gallery">
        <h2 style="text-align: right;">PROJECT DEPOT</h2>
        
        <!-- Row 1 -->
        <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 2rem;">
            
            <!-- Placeholder 1 -->
            <div class="card-3d">
                <div class="model-stage" style="height: 250px;">
                    <!-- TODO: Insert OBJ render for 'Mantra Films' or 'M-Tune' -->
                    <div class="label-3d">MTUNE_VISUALS.OBJ</div>
                </div>
                <h3>M-TUNE SERIES</h3>
                <p>Music videos: Samanalayage, Nariyage, Walahage.</p>
            </div>

            <!-- Placeholder 2 -->
            <div class="card-3d">
                <div class="model-stage" style="height: 250px;">
                    <!-- TODO: Insert OBJ render for 'Elephant House' Ads -->
                    <div class="label-3d">ELEPHANT_PROD.OBJ</div>
                </div>
                <h3>ORANGE COMMERCIALS</h3>
                <p>Wireman Switch, Elephant House, Popsicles.</p>
            </div>
        </div>

        <!-- Row 2 -->
        <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; margin-top: 2rem;">
            
            <!-- Placeholder 3 -->
            <div class="card-3d">
                <div class="model-stage" style="height: 250px;">
                    <!-- TODO: Insert OBJ render for Game Assets -->
                    <div class="label-3d">PANBATTA_GAME.OBJ</div>
                </div>
                <h3>GAME DESIGN</h3>
                <p>Assets and environments for Panbatta and Snow Ball.</p>
            </div>

            <!-- Placeholder 4 -->
            <div class="card-3d">
                <div class="model-stage" style="height: 250px;">
                    <!-- TODO: Insert OBJ render for Freelance / Cheqd -->
                    <div class="label-3d">CHEQD_ASSETS.OBJ</div>
                </div>
                <h3>INTERNATIONAL</h3>
                <p>Projects for Ideal Semiconductor (USA) & Cheqd (UK).</p>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer style="text-align: center; padding: 2rem; border-top: 1px solid rgba(255,255,255,0.1); color: var(--text-muted);">
        <p>&copy; 2024 MADHUKA SANDEEPA. SYSTEM ONLINE.</p>
    </footer>

</body>
</html>
