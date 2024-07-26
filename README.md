# Create-a-simple-personal-homepage-that-includes-essential-information-about-yourself
<!DOCTYPE html>
<html lang="en">
<head>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
<title>Renuka Nalluri</title>
<link rel="stylesheet" href="task1.css">
</head>
<body>
<header>
<div class="container">
<h1>Renuka Nalluri</h1>
<nav>
<ul>
<li><a href="#about" onclick="showSection('about')">About Me</a></li>
<li><a href="#portfolio" onclick="showSection('portfolio')">Portfolio</a></li>
<li><a href="#skills" onclick="showSection('skills')">Skills</a></li>
<li><a href="#contact" onclick="showSection('contact')">Contact</a></li>
</ul>
</nav>
</div>
</header>
<h2>Welcome to my personal homepage.</h2>
<img src="https://www.pushengage.com/wp-content/uploads/2022/02/Best-Website-Welcome-Message-Examples.png" alt="Default Image" id="default-image">
<main>
<div class="section" id="about">
<div class="container">
<h1>About Me</h1>
<p>My name is Renuka Nalluri</p>
<p>My father name is Srinivasarao Nalluri</p>
<p>My mother name is RajyaLakshmi Nalluri</p>
<p>I am from Ongole</p>
<p>I am a STUDENT</p>
<p>I am pursuing graduation at Qis college of Engineering and Technology|| Computer Science and Engineering</p>

</div>
</div>
<div class="section" id="portfolio">
<div class="container">
<h1>Portfolio</h1>
<p>I have done a internship of Python .</p>
</div>
</div>
<div class="section" id="skills">
<div class="container">
<h1>Skills</h1>
<h3>Qualifications:</h3>
<p>I am studying III B.Tech in QIS College of Engineering and Technology, Ongole.</p>
<p>I have completed my Intermediate in Sri Saraswathi Junior College,Ongole.</p>
<p>I have completed my schooling in Sivani High School, Ongole.</p>
<p>I have some basic knowledge of coding languages like HTML, CSS, JAVA, JS, PYTHON, C</p>
<p>I learnt the coding languages and certified by known platforms like GreatLearning, LinkedIn Learning, Sololearn, etc.</p>
</div>
</div>
<div class="section" id="contact">
<div class="container">
<h1>Contact</h1>
<h2>Via</h2>
<a href="https://www.linkedin.com/in/renuka-nalluri-0626b2274?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><i class="fab fa-linkedin"></i>LinkedIn</a>
<a href="https://www.instagram.com/renuka__nalluri?utm_source=qr&igsh=MW8wZG1neGhtNWVsNg==" target="_blank"><i class="fab fa-instagram"></i>Instagram</a>
<a href="https://wa.me/qr/7YGV4CNQCOMCC1" target="_blank"><i class="fab fa-whatsapp"></i>WhatsApp</a>
<a href="renukanalluri9@gmail.com"><i class="fas fa-envelope"></i>Email</a>
</div>
</div>
</main>
<footer>
<div class="container">
<p>&copy; Renuka Nalluri. All rights reserved.</p>
<p>Follow me on social media:</p>
<a href="https://www.linkedin.com/in/renuka-nalluri-0626b2274?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><i class="fab fa-linkedin"></i>LinkedIn</a>
<a href="https://www.instagram.com/renuka__nalluri?utm_source=qr&igsh=MW8wZG1neGhtNWVsNg==" target="_blank"><i class="fab fa-instagram"></i>Instagram</a>
<a href="https://wa.me/qr/7YGV4CNQCOMCC1" target="_blank"><i class="fab fa-whatsapp"></i>WhatsApp</a>
<a href="renukanalluri9@gmail.com"><i class="fas fa-envelope"></i>Email</a>
</div>
</footer>
<script>
    function showSection(sectionId) {
        const sections = document.querySelectorAll('.section');
        sections.forEach(section => {
            section.style.display = 'none';
        });

        const activeSection = document.getElementById(sectionId);
        activeSection.style.display = 'block';

        // Hide default image when a section is shown
        document.getElementById('default-image').style.display = 'none';
    }

    document.addEventListener('DOMContentLoaded', () => {
        // No section is shown by default
        document.querySelectorAll('.section').forEach(section => {
            section.style.display = 'none';
        });
    });
</script>
</body>
</html>


#css
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: chocolate;
    color: #333;
    display: flex;
    flex-direction: column;
    align-items: center;
    min-height: 100vh;
}
.container {
    width: 80%;
    margin: auto;
    overflow: hidden;
}
header {
    background: #333;
    color: #fff;
    padding-top: 30px;
    min-height: 70px;
    border-bottom: #c3d1d1 15px solid;
    width: 100%;
}
header h1 {
    text-align: center;
    margin: 0;
}
header nav {
    text-align: center;
    margin-top: 10px;
}
header nav ul {
    padding: 0;
    list-style: none;
}
header nav ul li {
    display: inline;
    margin: 0 15px;
}
header nav ul li a {
    color: #fff;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 16px;
    padding: 10px 20px;
    border-radius: 25px;
    background: rgba(158, 83, 83, 0.1);
    border: 2px solid transparent;
    transition: background 0.3s, transform 0.3s, color 0.3s, border-color 0.3s;
}
header nav ul li a:hover {
    background: rgb(11, 10, 10);
    color: red;
    border-color: rgb(7, 70, 70);
    transform: scale(1.1);
}
h2 {
    background: #fff;
    text-decoration: underline;
    font-style: italic;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    width: 600px;
    height: 35px;
    border-radius: 5px;
    text-align: center;
    margin: 20px 0;
}
#default-image {
    display: block;
    width: 500px;
    height: auto;
    margin: 20px 0;
}
main {
    flex-grow: 1;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 20px; 
}
.section {
    display: none;
    padding: 20px 0;
    background: #fff;
    margin: 20px 0;
    border-radius: 25px;
    width: 700px;
    text-align: center;
    transition: background-color 0.5s, color 0.5s;
}
.section h1, .section h2 {
    text-align: center;
    margin: 0 0 10px 0;
}
.section p {
    text-align: center;
    line-height: 1.6;
}
.section a {
    color: #333;
    text-align: center;
}
.social {
    text-align: center;
    padding: 20px;
}
.social a {
    margin: 0 10px;
    text-decoration: none;
    color: #333;
    font-size: 20px;
}
.social i {
    margin-right: 8px;
}
footer {
    text-align: center;
    padding: 20px 0;
    background: #333;
    color: #fff;
    width: 100%;
    position: relative;
}
footer a {
    color: aliceblue;
}
