# My-website
[IMG_6742](https://github.com/user-attachments/assets/366d77c6-8728-4a65-963c-7f2cea9ab2d2)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Anashe Mudhviwa- Aspiring Cyber Security specialist</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <header class="bg-primary text-white text-center py-5">
    <div class="container">
      <h1>Anashe Mudhuviwa</h1>
      <p class="lead">Cyber Security Analyst | Academic Institute of Excellence</p>
      <img src="IMG_6742.png" class="rounded-circle mt-3" alt="Anashe Mudhuviwa" width="150" height="150">
    </div>
  </header>

  <nav class="navbar navbar-expand-lg navbar-dark bg-dark sticky-top">
    <div class="container">
      <a class="navbar-brand" href="#">My Portfolio</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#about">About</a></li>
          <li class="nav-item"><a class="nav-link" href="#experience">Experience</a></li>
          <li class="nav-item"><a class="nav-link" href="#skills">Skills</a></li>
          <li class="nav-item"><a class="nav-link" href="#projects">Projects</a></li>
          <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
          <li class="nav-item"><a class="nav-link" href="https://github.com/#" target="_blank">GitHub</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <section id="about" class="py-5 bg-light">
    <div class="container">
      <h2 class="mb-4">About Me</h2>
      <p>
        I am a passionate first-year IT student at the Academic Institute of Excellence, currently learning the foundations of CyberSecurity.
      </p>
      <p>
        My goal is to become a CyberSecurity specialist and run my own CyberSecurity company 
      </p>
    </div>
  </section>

  <section id="experience" class="py-5">
    <div class="container">
      <h2 class="mb-4">Experience</h2>
      <h4>Student Projects - AIE</h4>
      <p>
        Working on mini-projects and assessments as part of my coursework, including basic web pages, console applications, and group assignments.
      </p>

      <h4>Self-Learning & Practice</h4>
      <p>
        I regularly use platforms like YouTube to reinforce class concepts and improve my practical skills in coding.
        I have 3+ years experience with virtual mechines with 2+ years pentration testing,Digital forensics,network scanning,vulnerability scanning and have built a home server
        I have ALL Certificates in CyberSecurity related course with Cisco accademy along side, ISC2 CyberSecurity certifcation, Linkedin CyberSecurity certifcation and currently working on getting my Comptia security+ and network+
      </p>
    </div>
  </section>

  <section id="skills" class="py-5 bg-light">
    <div class="container">
      <h2 class="mb-4">Skills</h2>
      <div class="row">
        <div class="col-md-6">
          <ul>
            <li>Penetration testing</li>
            <li>Port scanning</li>
            <li>Vulnerabiility scanning</li>
            <li>Navigate Virtual mechines</li>
          </ul>
        </div>
        <div class="col-md-6">
          <ul>
            <li>Microsoft Power BI (Intro)</li>
            <li>Kalilinux & ubuntu</li>
            <li>GitHub & Git</li>
            <li>Teamwork & Collaboration</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <section id="projects" class="py-5">
    <div class="container">
      <div class="mb-3">
      

      </div>
    </div>
  </section>

  <section id="contact" class="py-5 bg-light">
    <div class="container">
      <h2 class="mb-4">Contact Me</h2>
      <form id="contact-form">
        <div class="mb-3">
          <label for="name" class="form-label">Name:</label>
          <input type="text" class="form-control" id="name" name="name" required>
        </div>
        <div class="mb-3">
          <label for="email" class="form-label">Email:</label>
          <input type="email" class="form-control" id="email" name="email" required>
        </div>
        <div class="mb-3">
          <label for="message" class="form-label">Message:</label>
          <textarea class="form-control" id="message" name="message" rows="4" required></textarea>
        </div>
        <button type="submit" class="btn btn-primary">Send Message!</button>
      </form>
    </div>
  </section>

  <footer class="text-center text-white bg-dark py-3">
    <p class="mb-0">&copy; 2025 Anashe Mudhuviwa | IT Student @ AIE</p>
  </footer>

  <a href="#" class="btn btn-secondary position-fixed bottom-0 end-0 m-4" id="back-to-top">↑ Top</a>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
  <script src="script.js"></script>
</body>
</html>
{
	"folders": [
		{
			"path": "."
		}
	]
}
// JavaScript for back to top button
window.onscroll = function() {scrollFunction()};
function scrollFunction() {
    if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
        document.getElementById("back-to-top").style.display = "block";
    } else {
        document.getElementById("back-to-top").style.display = "none";
    }
}

document.getElementById("back-to-top").addEventListener("click", backToTop);

function backToTop() {
    document.body.scrollTop = 0;
    document.documentElement.scrollTop = 0;
}

// JavaScript for contact form submission
document.getElementById("contact-form").addEventListener("submit", function(event) {
    event.preventDefault(); // Prevent the default form submission behavior
    // You can add your code here to handle form submission, such as sending the form data to a server
    // For demonstration purposes, let's just log the form data to the console
    const formData = new FormData(this);
    for (const [name, value] of formData.entries()) {
        console.log(`${name}: ${value}`);
    }
    alert("Your message has been sent!"); // Display an alert after form submission
    this.reset(); // Reset the form fields after submission
});
//hosting , functionality of the contact form, 
/* CSS styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    margin-bottom: 80px; /* Added margin to prevent footer overlap */
}
header {
    background-color: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
    position: relative;
}
#profile-image {
    position: absolute;
    top: 20px;
    right: 20px;
    width: 100px;
    border-radius: 50%;
    border: 2px solid #fff;
}
nav {
    background-color: #f4f4f4;
    padding: 10px 0;
    text-align: center;
}
nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}
nav ul li {
    display: inline;
    margin-right: 20px;
}
nav ul li a {
    color: #333;
    text-decoration: none;
}
nav ul li a:hover {
    color: #000;
}
section {
    padding: 20px;
}
footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 20px;
    position: fixed;
    bottom: 0;
    width: 100%;
}
/* Back to top button */
#back-to-top {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: #333;
    color: #fff;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    display: none;
}
#back-to-top:hover {
    background-color: #555;
}
/* Contact form */
#contact-form {
    margin-top: 20px;
    background-color: #f4f4f4;
    padding: 20px;
    border-radius: 5px;
}
#contact-form label {
    display: block;
    margin-bottom: 10px;
}
#contact-form input[type="text"],
#contact-form input[type="email"],
#contact-form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-sizing: border-box;
}
#contact-form textarea {
    resize: vertical;
}
#contact-form button[type="submit"] {
    background-color: #333;
    color: #fff;
    border: none;
    padding: 10px 20px;
    border-radius: 5px;
    cursor: pointer;
}
#contact-form button[type="submit"]:hover {
    background-color: #555;
}

