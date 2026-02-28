<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Jesika Narvariya | Portfolio</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', sans-serif;
        }

        body {
            background: linear-gradient(to right, #e2e8f0, #f8fafc);
            color: #1e293b;
            line-height: 1.6;
        }

        header {
            background: linear-gradient(to right, #1e293b, #334155);
            color: white;
            padding: 60px 20px;
            text-align: center;
        }

        header h1 {
            font-size: 38px;
            margin-bottom: 10px;
        }

        header p {
            font-size: 18px;
            opacity: 0.9;
        }

        section {
            padding: 50px 20px;
            max-width: 900px;
            margin: auto;
        }

        h2 {
            margin-bottom: 20px;
            font-size: 26px;
            border-left: 5px solid #2563eb;
            padding-left: 10px;
        }

        .card {
            background: white;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.05);
        }

        ul {
            margin-top: 15px;
            padding-left: 20px;
        }

        li {
            margin-bottom: 10px;
        }

        .contact a {
            display: block;
            margin: 10px 0;
            text-decoration: none;
            color: #2563eb;
            font-weight: 500;
        }

        .contact a:hover {
            color: #1e40af;
        }

        footer {
            text-align: center;
            padding: 20px;
            background: #1e293b;
            color: white;
            margin-top: 40px;
        }

        @media (max-width: 600px) {
            header h1 {
                font-size: 28px;
            }
        }
    </style>
</head>

<body>

<header>
    <h1>Jesika Narvariya</h1>
    <p>Frontend Developer | Computer Science Student</p>
</header>

<section>
    <h2>About Me</h2>
    <div class="card">
        <p>
            Hello! I am Jesika Narvariya, a passionate Computer Science student 
            interested in web development and software engineering. 
            I enjoy building clean, responsive, and user-friendly interfaces 
            while continuously learning modern frontend technologies.
        </p>
    </div>
</section>

<section>
    <h2>Skills & Interests</h2>
    <div class="card">
        <ul>
            <li>HTML, CSS, JavaScript</li>
            <li>React.js (Basics)</li>
            <li>Responsive Web Design</li>
            <li>Problem Solving</li>
            <li>Frontend Development & UI Design</li>
        </ul>
    </div>
</section>

<section class="contact">
    <h2>Contact</h2>
    <div class="card">
        <a href="mailto:jesikan001@gmail.com">
            📧 Email: jesikan001@gmail.com
        </a>

        <a href="https://www.linkedin.com/in/jesika-narvariya" target="_blank">
            💼 LinkedIn: Jesika Narvariya
        </a>

        <a href="https://github.com/jesikanarvariya21" target="_blank">
            💻 GitHub: jesikanarvariya21
        </a>
    </div>
</section>

<footer>
    © 2026 Jesika Narvariya | All Rights Reserved
</footer>

</body>
</html>