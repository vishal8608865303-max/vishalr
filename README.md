<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Personal Resume Portfolio</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
    font-family:Arial, sans-serif;
}

body{
    background:#0f172a;
    color:white;
    line-height:1.6;
}

/* HEADER */
header{
    background:linear-gradient(135deg,#1e3a8a,#9333ea);
    padding:25px;
    text-align:center;
    animation:fadeIn 2s ease;
}

header h1{
    font-size:40px;
}

header p{
    margin-top:8px;
    font-size:18px;
}

/* NAVIGATION */
nav{
    background:#111827;
    padding:15px;
    position:sticky;
    top:0;
    z-index:1000;
}

nav ul{
    display:flex;
    justify-content:center;
    list-style:none;
    flex-wrap:wrap;
}

nav ul li{
    margin:10px 20px;
}

nav ul li a{
    color:white;
    text-decoration:none;
    font-weight:bold;
    transition:0.4s;
}

nav ul li a:hover{
    color:#38bdf8;
    transform:scale(1.1);
}

/* SECTION */
section{
    padding:60px 10%;
}

.section-title{
    font-size:35px;
    margin-bottom:20px;
    color:#38bdf8;
    border-left:5px solid #38bdf8;
    padding-left:15px;
}

/* ABOUT */
.about-container{
    display:flex;
    align-items:center;
    gap:40px;
    flex-wrap:wrap;
}

.about-container img{
    width:250px;
    height:250px;
    border-radius:50%;
    border:5px solid #38bdf8;
    transition:0.5s;
}

.about-container img:hover{
    transform:scale(1.05);
}

.about-text{
    flex:1;
}

/* CARDS */
.card-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.card{
    background:#1e293b;
    padding:25px;
    border-radius:15px;
    transition:0.4s;
}

.card:hover{
    transform:translateY(-10px);
    box-shadow:0 0 20px #38bdf8;
}

/* SKILLS */
.skill{
    margin-bottom:20px;
}

.skill-bar{
    background:#334155;
    border-radius:20px;
    overflow:hidden;
}

.skill-fill{
    height:15px;
    background:#38bdf8;
    border-radius:20px;
    animation:fillBar 2s ease;
}

.html{width:95%;}
.css{width:90%;}
.python{width:80%;}
.mysql{width:75%;}

/* TABLE */
table{
    width:100%;
    border-collapse:collapse;
    margin-top:20px;
}

table, th, td{
    border:1px solid white;
}

th{
    background:#2563eb;
}

th, td{
    padding:15px;
    text-align:center;
}

/* CONTACT */
.contact-links a{
    display:block;
    color:#38bdf8;
    margin:10px 0;
    text-decoration:none;
}

form{
    margin-top:20px;
}

input, textarea{
    width:100%;
    padding:12px;
    margin-bottom:15px;
    border:none;
    border-radius:10px;
}

button{
    padding:12px 25px;
    border:none;
    background:#38bdf8;
    color:white;
    font-size:16px;
    border-radius:10px;
    cursor:pointer;
    transition:0.4s;
}

button:hover{
    background:#2563eb;
    transform:scale(1.05);
}

/* FOOTER */
footer{
    text-align:center;
    padding:20px;
    background:#111827;
}

/* ANIMATIONS */
@keyframes fadeIn{
    from{
        opacity:0;
        transform:translateY(-30px);
    }
    to{
        opacity:1;
        transform:translateY(0);
    }
}

@keyframes fillBar{
    from{
        width:0;
    }
}
</style>
</head>

<body>

<header>
    <h1>Vishal</h1>
    <p>Roll No: 12345 | B.Sc Computer Science</p>
    <p>Batch: 2023 - 2026</p>
    <p>ABC College of Arts and Science</p>
</header>

<nav>
    <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#achievements">Achievements</a></li>
        <li><a href="#engagement">Engagement</a></li>
        <li><a href="#education">Education</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<section id="about">
    <h2 class="section-title">About Me</h2>

    <div class="about-container">
        <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e" alt="Profile">

        <div class="about-text">
            <p>
                Hello! I am <strong>Vishal</strong>, a passionate Computer Science student interested in web development and UI design.
            </p>
        </div>
    </div>
</section>

<section id="projects">
    <h2 class="section-title">Projects</h2>

    <div class="card-container">
        <div class="card">
            <h3>Portfolio Website</h3>
            <p>Created using HTML and CSS.</p>
        </div>

        <div class="card">
            <h3>Student Management System</h3>
            <p>Developed using Python and MySQL.</p>
        </div>
    </div>
</section>

<section id="skills">
    <h2 class="section-title">Skills</h2>

    <div class="skill">
        <h3>HTML</h3>
        <div class="skill-bar">
            <div class="skill-fill html"></div>
        </div>
    </div>

    <div class="skill">
        <h3>CSS</h3>
        <div class="skill-bar">
            <div class="skill-fill css"></div>
        </div>
    </div>

    <div class="skill">
        <h3>Python</h3>
        <div class="skill-bar">
            <div class="skill-fill python"></div>
        </div>
    </div>
</section>

<section id="education">
    <h2 class="section-title">Education</h2>

    <table>
        <tr>
            <th>Qualification</th>
            <th>Institution</th>
            <th>Year</th>
        </tr>

        <tr>
            <td>B.Sc Computer Science</td>
            <td>ABC College</td>
            <td>2023 - 2026</td>
        </tr>
    </table>
</section>

<section id="contact">
    <h2 class="section-title">Contact</h2>

    <div class="contact-links">
        <a href="mailto:vishal@gmail.com">Email: vishal@gmail.com</a>
        <a href="#">Phone: +91 9876543210</a>
    </div>

    <form>
        <input type="text" placeholder="Enter Your Name" required>
        <input type="email" placeholder="Enter Your Email" required>
        <textarea rows="6" placeholder="Enter Your Message"></textarea>
        <button type="submit">Send Message</button>
    </form>
</section>

<footer>
    <p>© 2026 Vishal | Personal Resume Website</p>
</footer>

</body>
</html>