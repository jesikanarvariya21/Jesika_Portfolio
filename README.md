<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Jesika Narvariya | Portfolio</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <nav class="navbar">
        <h1 class="logo">Jesika Narvariya</h1>
        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <header class="hero">
        <h2>Hello, I'm Jesika 👋</h2>
        <p>Electronics and Communication Engineering Student</p>
        <button onclick="scrollToContact()">Contact Me</button>
    </header>

    <section id="about" class="section">
        <h2>About Me</h2>
        <p>
            I am Jesika Narvariya, a dedicated Electronics and Communication Engineering student 
            with a strong interest in technology and frontend development. 
            I am passionate about learning new skills and building modern, user-friendly websites.
        </p>
    </section>

    <section id="skills" class="section">
        <h2>Skills & Areas of Interest</h2>
        <div class="skills-container">
            <div class="skill-card">HTML</div>
            <div class="skill-card">CSS</div>
            <div class="skill-card">JavaScript</div>
            <div class="skill-card">Frontend Development</div>
            <div class="skill-card">UI/UX Basics</div>
            <div class="skill-card">Electronics & Communication</div>
        </div>
    </section>

    <section id="contact" class="section contact-section">
        <h2>Contact Information</h2>
        <p><strong>Email:</strong> jesikan001@gmail.com</p>
        <p><strong>LinkedIn:</strong> Jesika Narvariya</p>
        <p><strong>GitHub:</strong> jesikanarvariya21</p>
    </section>

    <footer>
        <p>© 2026 Jesika Narvariya | All Rights Reserved</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', sans-serif;
}

body {
    background: #f4f7fa;
    color: #333;
    line-height: 1.6;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background: #0f172a;
    padding: 15px 40px;
    color: white;
}

.logo {
    font-size: 20px;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin-left: 20px;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-size: 14px;
}

.nav-links a:hover {
    color: #38bdf8;
}

.hero {
    text-align: center;
    padding: 80px 20px;
    background: linear-gradient(to right, #0f172a, #1e293b);
    color: white;
}

.hero button {
    margin-top: 20px;
    padding: 10px 20px;
    border: none;
    background: #38bdf8;
    color: white;
    cursor: pointer;
    border-radius: 5px;
}

.hero button:hover {
    background: #0ea5e9;
}

.section {
    padding: 60px 20px;
    max-width: 1000px;
    margin: auto;
    text-align: center;
}

.section h2 {
    margin-bottom: 20px;
    color: #0f172a;
}

.skills-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
}

.skill-card {
    background: white;
    padding: 15px 25px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    font-weight: bold;
}

.contact-section p {
    margin: 10px 0;
}

footer {
    text-align: center;
    padding: 15px;
    background: #0f172a;
    color: white;
}
function scrollToContact() {
    document.getElementById("contact").scrollIntoView({
        behavior: "smooth"
    });
}