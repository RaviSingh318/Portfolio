<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ravi Singh | Software Tester</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<script src="https://unpkg.com/scrollreveal"></script>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
    scroll-behavior:smooth;
}

body{
    background:linear-gradient(135deg,#0f172a,#1e293b);
    color:#fff;
}

nav{
    position:fixed;
    width:100%;
    padding:15px 10%;
    display:flex;
    justify-content:space-between;
    background:rgba(0,0,0,0.3);
    backdrop-filter:blur(10px);
    z-index:1000;
}

nav a{
    color:#fff;
    text-decoration:none;
    margin-left:20px;
    font-weight:500;
}

section{
    min-height:100vh;
    padding:100px 10%;
    display:flex;
    flex-direction:column;
    justify-content:center;
}

.hero{
    text-align:center;
}

.hero h1{
    font-size:50px;
    background:linear-gradient(90deg,#38bdf8,#818cf8);
    -webkit-background-clip:text;
    color:transparent;
}

.hero h2{
    margin-top:15px;
    font-weight:400;
    color:#cbd5e1;
}

.btn{
    margin-top:25px;
    padding:12px 25px;
    border:none;
    background:linear-gradient(90deg,#38bdf8,#818cf8);
    color:#000;
    font-weight:600;
    border-radius:30px;
    cursor:pointer;
    text-decoration:none;
}

.glass{
    background:rgba(255,255,255,0.05);
    padding:25px;
    border-radius:15px;
    backdrop-filter:blur(12px);
    margin-top:25px;
    box-shadow:0 8px 32px rgba(0,0,0,0.4);
}

h2.section-title{
    font-size:32px;
    margin-bottom:20px;
    color:#38bdf8;
}

.skills span{
    display:inline-block;
    background:#1e293b;
    padding:8px 15px;
    border-radius:20px;
    margin:5px;
    font-size:14px;
}

footer{
    text-align:center;
    padding:20px;
    background:#111827;
}

@media(max-width:768px){
    .hero h1{font-size:35px;}
}
</style>
</head>

<body>

<nav>
    <div><strong>Ravi Singh</strong></div>
    <div>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
    </div>
</nav>

<section class="hero">
    <h1>Ravi Singh</h1>
    <h2><span id="typing"></span></h2>
    <a href="26 Feb Resume.pdf" download class="btn">Download Resume</a>
</section>

<section id="about">
    <h2 class="section-title">About Me</h2>
    <div class="glass">
        IT Graduate and passionate Software Tester with hands-on experience in
        Manual, Functional, Regression and API Testing.
        Strong knowledge of SDLC, STLC and Agile methodologies.
        Dedicated to delivering high-quality software solutions.
    </div>
</section>

<section id="skills">
    <h2 class="section-title">Skills</h2>
    <div class="glass skills">
        <span>Manual Testing</span>
        <span>Functional Testing</span>
        <span>UAT</span>
        <span>SDLC</span>
        <span>STLC</span>
        <span>Agile Scrum</span>
        <span>Jira</span>
        <span>Bugzilla</span>
        <span>Azure DevOps</span>
        <span>Postman</span>
        <span>JMeter</span>
        <span>Python</span>
        <span>JavaScript</span>
        <span>GitHub</span>
    </div>
</section>

<section id="projects">
    <h2 class="section-title">Projects</h2>

    <div class="glass">
        <h3>OpenCart Website Testing</h3>
        <p>End-to-end functional testing for e-commerce workflows including registration, cart, checkout & bug tracking.</p>
    </div>

    <div class="glass">
        <h3>AbleSpace Student Data Platform</h3>
        <p>Manual UI/UX testing, goal management validation & defect documentation.</p>
    </div>

    <div class="glass">
        <h3>Kredily HRMS Application</h3>
        <p>Leave request module testing with boundary & negative test cases execution.</p>
    </div>
</section>

<section id="contact">
    <h2 class="section-title">Contact</h2>
    <div class="glass">
        <p>Email: ravirajput0990@gmail.com</p>
        <p>Phone: +91-7977859240</p>
        <p>Location: Navi Mumbai, Maharashtra</p>
        <p>
            <a href="https://www.linkedin.com/in/ravisingh831/" target="_blank">LinkedIn</a> |
            <a href="https://github.com/RaviSingh318" target="_blank">GitHub</a>
        </p>
    </div>
</section>

<footer>
    © 2026 Ravi Singh | Software Tester
</footer>

<script>
// Typing Effect
const text = ["Software Tester", "Manual & API Testing", "QA Enthusiast"];
let count = 0;
let index = 0;
let currentText = "";
let letter = "";

(function type(){
    if(count === text.length){
        count = 0;
    }
    currentText = text[count];
    letter = currentText.slice(0, ++index);
    document.getElementById("typing").textContent = letter;
    if(letter.length === currentText.length){
        count++;
        index = 0;
        setTimeout(type,1000);
    }else{
        setTimeout(type,100);
    }
})();

// Scroll Reveal Animation
ScrollReveal().reveal('.glass',{
    delay:200,
    distance:'40px',
    origin:'bottom',
    duration:1000,
    reset:false
});
</script>

</body>
</html>
