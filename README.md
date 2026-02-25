# Jesika_Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
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
        <h2><span id="typing"></span></h2>
        <div class="hero-buttons">
            <a href="#contact" class="btn">Connect With Me</a>
            <a href="resume.pdf" class="btn-outline" download>Download Resume</a>
        </div>
    </div>
</header>

<section id="about" class="section reveal">
    <h2>About Me</h2>
    <p>
        I am an Electronics and Communication Engineering student passionate about
        C programming and digital creativity. I enjoy solving real-world problems,
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
        <div class="card">C Programming Mini Projects</div>
        <div class="card">Creative Editing Showcase</div>
    </div>
</section>

<section id="contact" class="section reveal">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:jesikan001@gmail.com">jesikan001@gmail.com</a></p>
    <p>LinkedIn:
        <a href="https://www.linkedin.com/in/jesika-narvariya" target="_blank">
            Jesika Narvariya
        </a>
    </p>
    <p>GitHub:
        <a href="https://github.com/jesikanarvariya21" target="_blank">
            jesikanarvariya21
        </a>
    </p>
</section>

<footer>
    <p>© 2026 Jesika Narvariya | All Rights Reserved</p>
</footer>

<script src="script.js"></script>
</body>
</html>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:'Segoe UI',sans-serif;
    background:#0f172a;
    color:white;
    scroll-behavior:smooth;
}

/* Navbar */
nav{
    position:fixed;
    width:100%;
    display:flex;
    justify-content:space-between;
    padding:20px 60px;
    background:rgba(15,23,42,0.9);
    backdrop-filter:blur(10px);
    z-index:1000;
}

nav ul{
    display:flex;
    list-style:none;
    gap:30px;
}

nav a{
    text-decoration:none;
    color:white;
    transition:0.3s;
}

nav a:hover{
    color:#38bdf8;
}

/* Hero */
.hero{
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    background:linear-gradient(135deg,#1e3a8a,#0f172a);
    text-align:center;
}

.hero-content{
    background:rgba(255,255,255,0.08);
    padding:60px;
    border-radius:20px;
    backdrop-filter:blur(15px);
}

.hero h1{
    font-size:48px;
}

.hero h2{
    margin-top:15px;
    color:#38bdf8;
}

.hero-buttons{
    margin-top:25px;
}

.btn, .btn-outline{
    padding:10px 25px;
    margin:10px;
    border-radius:25px;
    text-decoration:none;
    font-weight:bold;
    transition:0.3s;
}

.btn{
    background:#38bdf8;
    color:black;
}

.btn:hover{
    background:white;
}

.btn-outline{
    border:2px solid #38bdf8;
    color:#38bdf8;
}

.btn-outline:hover{
    background:#38bdf8;
    color:black;
}

/* Sections */
.section{
    padding:100px 20px;
    text-align:center;
}

.section h2{
    margin-bottom:30px;
    font-size:32px;
    color:#38bdf8;
}

.cards{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;
    gap:20px;
}

.card{
    background:#1e293b;
    padding:20px 30px;
    border-radius:15px;
    transition:0.4s;
}

.card:hover{
    transform:translateY(-10px);
    background:#334155;
}

a{
    color:#38bdf8;
    text-decoration:none;
}

footer{
    padding:20px;
    background:#0f172a;
}

/* Scroll Reveal */
.reveal{
    opacity:0;
    transform:translateY(60px);
    transition:1s ease;
}

.reveal.active{
    opacity:1;
    transform:translateY(0);
}
// Typing Effect
const text = "Electronics & Communication Engineer | C Programmer | Creative Editor";
let index = 0;

function type() {
    if (index < text.length) {
        document.getElementById("typing").innerHTML += text.charAt(index);
        index++;
        setTimeout(type, 50);
    }
}
window.onload = type;

// Scroll Reveal
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
