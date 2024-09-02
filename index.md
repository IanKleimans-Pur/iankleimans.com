<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ian Kleimans - Industrial Engineering Student</title>
    <style>
        :root {
            --primary-color: #3498db;
            --secondary-color: #2c3e50;
            --text-color: #333;
            --background-color: #f4f4f4;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--background-color);
        }
        .container {
            max-width: 1100px;
            margin: auto;
            overflow: hidden;
            padding: 0 2rem;
        }
        header {
            background-color: var(--primary-color);
            color: #fff;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        header h1 {
            font-size: 1.5rem;
        }
        nav ul {
            display: flex;
            list-style-type: none;
        }
        nav ul li {
            padding: 0 1rem;
        }
        nav ul li a {
            color: #fff;
            text-decoration: none;
        }
        main {
            padding: 6rem 0 3rem;
        }
        section {
            padding: 3rem 0;
        }
        h2 {
            color: var(--secondary-color);
            margin-bottom: 1rem;
        }
        .btn {
            display: inline-block;
            background: var(--primary-color);
            color: #fff;
            padding: 0.5rem 1rem;
            border: none;
            cursor: pointer;
            font-size: 1rem;
            text-decoration: none;
            transition: opacity 0.2s ease-in;
        }
        .btn:hover {
            opacity: 0.8;
        }
        .project {
            background: #fff;
            border-radius: 5px;
            padding: 1rem;
            margin-bottom: 1rem;
        }
        .skills ul {
            list-style-type: none;
            display: flex;
            flex-wrap: wrap;
        }
        .skills ul li {
            background: var(--secondary-color);
            color: #fff;
            padding: 0.5rem;
            margin: 0.5rem;
            border-radius: 5px;
        }
        footer {
            background: var(--secondary-color);
            color: #fff;
            text-align: center;
            padding: 1rem 0;
        }
        @media (max-width: 700px) {
            header .container {
                flex-direction: column;
            }
            nav ul {
                margin-top: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Ian Kleimans</h1>
            <nav>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#experience">Experience</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        <section id="about">
            <h2>About Me</h2>
            <p>I'm a passionate Industrial Engineering student at Purdue University, with a minor in Economics. I'm dedicated to leveraging technology and data analysis to create innovative solutions.</p>
            <a href="Ian-Kleimans_Resume.pdf" class="btn" target="_blank">View Full Resume</a>
        </section>

        <section id="projects">
            <h2>Projects</h2>
            <div class="project">
                <h3>Compute Tracker</h3>
                <p>A GPU tracking website to monitor compute power of leading AI companies.</p>
                <a href="http://computetracker.com/" class="btn" target="_blank">View Project</a>
            </div>
            <div class="project">
                <h3>SY753W Project</h3>
                <p>An innovative project showcasing data analysis and visualization techniques.</p>
                <a href="https://sy753w.csb.app/" class="btn" target="_blank">View Project</a>
            </div>
        </section>

        <section id="skills" class="skills">
            <h2>Skills</h2>
            <ul>
                <li>Python</li>
                <li>HTML</li>
                <li>JavaScript</li>
                <li>MATLAB</li>
                <li>AutoCAD</li>
                <li>SQL</li>
                <li>Data Analysis</li>
                <li>Project Management</li>
            </ul>
        </section>

        <section id="experience">
            <h2>Experience</h2>
            <div class="project">
                <h3>Market Research Analyst - Delta EM Advisors LTD</h3>
                <p>Conducted market research and analysis to support investment strategies for various funds. Led a team in evaluating financial databases and incorporating industry reports to identify investment opportunities.</p>
            </div>
            <div class="project">
                <h3>Founder & Vice President - Argentine and Uruguayan Club at Purdue University (ARGURU)</h3>
                <p>Organized events, cultural gatherings, and developed a mentorship program for upcoming first-year students to adjust faster with the university system.</p>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2024 Ian Kleimans. All rights reserved.</p>
        </div>
    </footer>

    <script>
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
