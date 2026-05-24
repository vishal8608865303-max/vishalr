<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vishal Portfolio</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#f4f4f4;
    color:#333;
    scroll-behavior:smooth;
}

header{
    background:linear-gradient(to right,#141e30,#243b55);
    color:white;
    padding:30px;
    text-align:center;
    animation:fadeIn 2s;
}

header h1{
    font-size:40px;
}

nav{
    background:#111;
    padding:15px;
    text-align:center;
    position:sticky;
    top:0;
}

nav a{
    color:white;
    text-decoration:none;
    margin:15px;
    font-weight:bold;
    transition:0.3s;
}

nav a:hover{
    color:yellow;
    font-size:18px;
}

section{
    padding:40px;
}

.container{
    max-width:1100px;
    margin:auto;
}

.card{
    background:white;
    padding:25px;
    margin-top:20px;
    border-radius:10px;
    box-shadow:0 0 10px rgba(0,0,0,0.2);
    transition:0.5s;
}

.card:hover{
    transform:scale(1.03);
}

h2{
    color:#243b55;
    margin-bottom:15px;
}

ul li{
    margin:10px 0;
}

table{
    width:100%;
    border-collapse:collapse;
    margin-top:15px;
}

table,th,td{
    border:1px solid #555;
}

th{
    background:#243b55;
    color:white;
}

th,td{
    padding:12px;
    text-align:center;
}

.skill{
    margin:15px 0;
}

.bar{
    background:#ddd;
    border-radius:20px;
    overflow:hidden;
}

.progress{
    height:20px;
    background:#243b55;
    animation:load 3s;
}

form input, form textarea{
    width:100%;
    padding:12px;
    margin:10px 0;
    border-radius:5px;
    border:1px solid #aaa;
}

button{
    background:#243b55;
    color:white;
    padding:12px 25px;
    border:none;
    border-radius:5px;
    cursor:pointer;
    transition:0.3s;
}

button:hover{
    background:black;
}

footer{
    background:#111;
    color:white;
    text-align:center;
    padding:20px;
    margin-top:30px;
}

img{
    width:180px;
    border-radius:50%;
    margin-top:15px;
    border:5px solid white;
}

iframe{
    width:100%;
    height:300px;
    border:none;
    margin-top:20px;
}

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

@keyframes load{
    from{
        width:0;
    }
}

</style>
</head>

<body>

<header>
    <h1>Vishal M</h1>
    <p>Roll No: S24422</p>
    <p>Bachelor Of Computer Application (BCA)</p>
    <p>Batch: 2024 - 2027</p>
    <p>Cardamom Planters’ Association College</p>

    <img src="https://cdn-icons-png.flaticon.com/512/3135/3135715.png">
</header>

<nav>
    <a href="#about">About</a>
    <a href="#experience">Experience</a>
    <a href="#projects">Projects</a>
    <a href="#skills">Skills</a>
    <a href="#education">Education</a>
    <a href="#contact">Contact</a>
</nav>

<section id="about">
<div class="container">
<div class="card">
    <h2>About Me</h2>
    <p>
        I am Vishal M, a passionate BCA student interested in Full Stack Web Development,
        Python Programming, UI Design, and Software Development. I enjoy creating modern
        websites and learning new technologies.
    </p>
</div>
</div>
</section>

<section id="experience">
<div class="container">
<div class="card">
    <h2>Experience</h2>

    <ul>
        <li>Completed Virtual Internship on Full Stack Web Development</li>
        <li>Created personal portfolio websites using HTML and CSS</li>
        <li>Participated in coding workshops and seminars</li>
    </ul>

</div>
</div>
</section>

<section id="projects">
<div class="container">
<div class="card">
    <h2>Projects</h2>

    <h3>Personal Portfolio Website</h3>
    <p>
        Developed a responsive portfolio website using HTML and CSS.
    </p>

    <br>

    <h3>Student Management System</h3>
    <p>
        Built a mini student database application using Python.
    </p>

</div>
</div>
</section>

<section id="skills">
<div class="container">
<div class="card">

    <h2>Skills</h2>

    <div class="skill">
        <p>HTML</p>
        <div class="bar">
            <div class="progress" style="width:90%"></div>
        </div>
    </div>

    <div class="skill">
        <p>CSS</p>
        <div class="bar">
            <div class="progress" style="width:85%"></div>
        </div>
    </div>

    <div class="skill">
        <p>Python</p>
        <div class="bar">
            <div class="progress" style="width:80%"></div>
        </div>
    </div>

    <div class="skill">
        <p>Django</p>
        <div class="bar">
            <div class="progress" style="width:70%"></div>
        </div>
    </div>

</div>
</div>
</section>

<section id="education">
<div class="container">
<div class="card">

    <h2>Education</h2>

    <table>
        <tr>
            <th>Qualification</th>
            <th>Institution</th>
            <th>Year</th>
            <th>Grade</th>
        </tr>

        <tr>
            <td>BCA</td>
            <td>Cardamom Planters’ Association College</td>
            <td>2024 - 2027</td>
            <td>8.5 CGPA</td>
        </tr>

        <tr>
            <td>12th</td>
            <td>State Board</td>
            <td>2024</td>
            <td>85%</td>
        </tr>

        <tr>
            <td>10th</td>
            <td>State Board</td>
            <td>2022</td>
            <td>90%</td>
        </tr>

    </table>

</div>
</div>
</section>

<section id="contact">
<div class="container">
<div class="card">

    <h2>Contact Me</h2>

    <p><strong>Email:</strong> vishal@gmail.com</p>
    <p><strong>Phone:</strong> 9876543210</p>
    <p><strong>GitHub:</strong> github.com/vishal</p>
    <p><strong>LinkedIn:</strong> linkedin.com/in/vishal</p>

    <br>

    <form>
        <input type="text" placeholder="Enter Your Name" required>

        <input type="email" placeholder="Enter Your Email" required>

        <textarea rows="5" placeholder="Enter Your Message"></textarea>

        <button type="submit">Send Message</button>
    </form>

    <iframe 
    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3916.219187253982!2d76.9686!3d10.9983!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3ba859b9c63f4b53%3A0x2b0f6f8e7f4d9b8!2sCoimbatore!5e0!3m2!1sen!2sin!4v1716530000000">
    </iframe>

</div>
</div>
</section>

<footer>
    <p>© 2026 Vishal M | Personal Portfolio Website</p>
</footer>

</body>
</html>