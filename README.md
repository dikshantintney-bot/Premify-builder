<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premify</title>

    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: #0e0f10;
            color: white;
        }

        header {
            padding: 20px 10%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: transparent;
        }

        .logo {
            font-size: 28px;
            letter-spacing: 1px;
            font-weight: bold;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            font-size: 16px;
            opacity: 0.8;
            transition: 0.3s;
        }

        nav a:hover {
            opacity: 1;
        }

        /* Hero Section */
        .hero {
            padding: 100px 10%;
            text-align: center;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            animation: fadeIn 1.2s ease;
        }

        .hero p {
            font-size: 20px;
            opacity: 0.85;
            max-width: 700px;
            margin: 0 auto;
        }

        .hero button {
            margin-top: 35px;
            padding: 14px 28px;
            background: #4b82ff;
            border: none;
            border-radius: 8px;
            font-size: 18px;
            color: white;
            cursor: pointer;
            transition: 0.3s;
        }

        .hero button:hover {
            background: #3464d7;
        }

        /* Features */
        .features {
            padding: 80px 10%;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 30px;
        }

        .feature-box {
            background: #181a1d;
            padding: 30px;
            border-radius: 12px;
            transition: 0.3s;
        }

        .feature-box:hover {
            transform: translateY(-5px);
            background: #1f2226;
        }

        .feature-box h3 {
            margin-bottom: 12px;
            font-size: 22px;
        }

        .feature-box p {
            opacity: 0.7;
        }

        /* Footer */
        footer {
            padding: 30px;
            text-align: center;
            opacity: 0.7;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>

<body>

<header>
    <div class="logo">Premify</div>
    <nav>
        <a href="#features">Features</a>
        <a href="#download">Download</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero">
    <h1>Design. Build. Export. Instantly.</h1>
    <p>
        Premify is a next-generation GUI builder that lets developers visually create applications 
        and instantly export production-ready code in multiple languages — faster, cleaner, and smarter than ever.
    </p>
    <button onclick="scrollToFeatures()">Explore Features</button>
</section>

<section id="features" class="features">
    <div class="feature-box">
        <h3>Live Visual Editing</h3>
        <p>Drag, resize, configure — every change updates instantly with pixel-perfect precision.</p>
    </div>

    <div class="feature-box">
        <h3>Multi-Language Export</h3>
        <p>Generate clean source code for JavaFX, HTML/CSS/JS, and more coming soon.</p>
    </div>

    <div class="feature-box">
        <h3>Smart Layout Rules</h3>
        <p>Your UI never breaks. Built-in validation prevents invalid properties and layout mistakes.</p>
    </div>

    <div class="feature-box">
        <h3>Component Intelligence</h3>
        <p>Automatic suggestions for alignment, spacing, sizing, and structure.</p>
    </div>
</section>

<footer>
    © 2025 Premify — Crafted with passion.
</footer>

<script>
    function scrollToFeatures() {
        document.getElementById("features").scrollIntoView({ behavior: "smooth" });
    }
</script>

</body>
</html>
