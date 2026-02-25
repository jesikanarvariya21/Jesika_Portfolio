<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Jesika Narvariya | Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<nav>
    <div class="logo">Jesika</div>
    <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<header class="hero">
    <div class="hero-content">
        <h1>Jesika Narvariya</h1>
        <p>Electronics & Communication Engineer | C Programmer | Creative Editor</p>
        <a href="#contact" class="btn">Connect With Me</a>
    </div>
</header>

<section id="about" class="section reveal">
    <h2>About Me</h2>
    <p>
        I am an Electronics and Communication Engineering student passionate about 
        C programming and digital creativity. I enjoy solving problems, 
        learning emerging technologies, and building meaningful digital experiences.
    </p>
</section>

<section id="skills" class="section reveal">
    <h2>Skills</h2>
    <div class="cards">
        <div class="card">C Programming</div>
        <div class="card">Problem Solving</div>
        <div class="card">Video Editing</div>
        <div class="card">Creative Design</div>
    </div>
</section>

<section id="projects" class="section reveal">
    <h2>Projects</h2>
    <div class="cards">
        <div class="card">Student Portfolio Website</div>
        <div class="card">Basic C Programming Projects</div>
        <div class="card">Creative Editing Showcase</div>
    </div>
</section>

<section id="contact" class="section reveal">
    <h2>Contact</h2>
    <p>Email: your.email@example.com</p>
    <p>LinkedIn: linkedin.com/in/yourprofile</p>
    <p>GitHub: github.com/yourusername</p>
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
}

body {
    font-family: 'Segoe UI', sans-serif;
    background: #0f172a;
    color: white;
    scroll-behavior: smooth;
}

nav {
    position: fixed;
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding: 20px 60px;
    background: rgba(15, 23, 42, 0.9);
    backdrop-filter: blur(10px);
}

nav ul {
    display: flex;
    list-style: none;
    gap: 30px;
}

nav a {
    text-decoration: none;
    color: white;
    transition: 0.3s;
}

nav a:hover {
    color: #38bdf8;
}

.hero {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #1e3a8a, #0f172a);
    text-align: center;
}

.hero-content {
    background: rgba(255,255,255,0.1);
    padding: 50px;
    border-radius: 20px;
    backdrop-filter: blur(15px);
}

.hero h1 {
    font-size: 48px;
}

.hero p {
    margin: 20px 0;
}

.btn {
    padding: 10px 25px;
    background: #38bdf8;
    color: black;
    text-decoration: none;
    border-radius: 25px;
    font-weight: bold;
    transition: 0.3s;
}

.btn:hover {
    background: white;
}

.section {
    padding: 100px 20px;
    text-align: center;
}

.section h2 {
    margin-bottom: 30px;
    font-size: 32px;
    color: #38bdf8;
}

.cards {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
}

.card {
    background: #1e293b;
    padding: 20px 30px;
    border-radius: 15px;
    transition: 0.4s;
}

.card:hover {
    transform: translateY(-10px);
    background: #334155;
}

footer {
    padding: 20px;
    background: #0f172a;
    text-align: center;
}

/* Scroll Reveal Animation */
.reveal {
    opacity: 0;
    transform: translateY(60px);
    transition: 1s ease;
}

.reveal.active {
    opacity: 1;
    transform: translateY(0);
}
function reveal() {
    let reveals = document.querySelectorAll(".reveal");

    reveals.forEach((element) => {
        let windowHeight = window.innerHeight;
        let elementTop = element.getBoundingClientRect().top;
        let visible = 150;

        if (elementTop < windowHeight - visible) {
            element.classList.add("active");
        }
    });
}

window.addEventListener("scroll", reveal);