---
permalink: /test/
title: "👋🏼 Hello there, I'm Debojjal (Deb)!"
author_profile: true
redirect_from: 
  - /test/
  - /test.html
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Debojjal (Deb) - Portfolio</title>
  <!-- AOS Library -->
  <link href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css" rel="stylesheet">
  <style>
    /* Global Styles */
    body {
      font-family: "Times New Roman", Times, serif;
      font-size: 16px;
      color: #333;
      line-height: 1.6;
      margin: 0;
      padding: 0;
      background: linear-gradient(-45deg, #f5f5f5, #e0e0e0);
      background-size: 400% 400%;
      animation: gradient 15s ease infinite;
    }

    @keyframes gradient {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    a {
      color: #014552;
      text-decoration: none;
      transition: color 0.3s ease;
    }

    a:hover {
      color: #ff6347;
    }

    h1, h2, h3, h4, h5, h6 {
      margin-top: 24px;
      margin-bottom: 16px;
      font-weight: 600;
      line-height: 1.25;
    }

    /* Header Animation */
    .typewriter {
      overflow: hidden;
      border-right: .15em solid #014552;
      white-space: nowrap;
      margin: 0 auto;
      letter-spacing: .15em;
      animation: typing 3.5s steps(40, end), blink-caret .75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink-caret {
      from, to { border-color: transparent; }
      50% { border-color: #014552; }
    }

    /* Progress Bar */
    .progress-container {
      width: 100%;
      height: 5px;
      background: #ccc;
      position: fixed;
      top: 0;
      left: 0;
      z-index: 1000;
    }

    .progress-bar {
      height: 5px;
      background: #014552;
      width: 0%;
    }

    /* Sections */
    section {
      padding: 60px 20px;
      max-width: 800px;
      margin: 0 auto;
    }

    /* Floating Image */
    .floating {
      animation: float 3s ease-in-out infinite;
    }

    @keyframes float {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-20px); }
      100% { transform: translateY(0px); }
    }

    /* Buttons */
    .button {
      background-color: #014552;
      color: white;
      padding: 10px 20px;
      border-radius: 5px;
      transition: background-color 0.3s ease;
      display: inline-block;
    }

    .button:hover {
      background-color: #ff6347;
    }
  </style>
</head>
<body>
  <!-- Progress Bar -->
  <div class="progress-container">
    <div class="progress-bar" id="myBar"></div>
  </div>

  <!-- Header -->
  <header style="text-align: center; padding: 100px 20px;">
    <h1 class="typewriter" data-aos="fade-up">👋🏼 Hello there, I'm Debojjal (Deb)!</h1>
    <p data-aos="fade-up" data-aos-delay="200">Welcome to my personal website. Scroll down to learn more about me!</p>
  </header>

  <!-- About Section -->
  <section data-aos="fade-up">
    <h2>About Me</h2>
    <p>
      Hi! I'm currently a graduate student specializing in <a href="https://www.caee.utexas.edu/research/research-areas/transportation-engineering">Transportation Engineering</a> at the <a href="https://www.caee.utexas.edu/">Department of Civil, Architectural, and Environmental Engineering</a>, <a href="https://www.utexas.edu/">University of Texas at Austin</a>. My academic journey began with a <a href="https://ug.iisc.ac.in/">BS (research)</a> degree from the <a href="https://iisc.ac.in/">Indian Institute of Science (IISc), Bangalore</a>, where I majored in Earth & Environmental Science along with a minor in Mathematics.
    </p>
    <img src="https://via.placeholder.com/400" alt="Profile Image" class="floating" style="width: 100%; max-width: 400px; margin: 20px auto; display: block;">
  </section>

  <!-- Education Section -->
  <section data-aos="fade-up">
    <h2>Education</h2>
    <p>
      <strong>Master of Science in Engineering (M.S.E)</strong> - Aug 2023 -- Fall, 2024 (Expected)<br>
      <em>Major:</em> Transportation Engineering; <em>Minor:</em> Industrial Engineering and Operations Research, <a href="https://www.utexas.edu/">UT Austin</a><br>
      <em>Advisor:</em> <a href="https://sboyles.github.io/">Prof. Stephen Boyles</a>
    </p>
    <p>
      <strong>Bachelor of Science (B.S. by Research)</strong> - Aug 2019 -- May, 2023<br>
      <em>Major:</em> Earth and Environmental Science; <em>Minor:</em> Mathematics, <a href="https://iisc.ac.in/">IISc, Bengaluru</a><br>
      <em>Awards:</em> Gold Medal for highest GPA in major, Highest project grade, First Class Distinction<br>
      <em>Thesis:</em> Energy Efficient and Safe Routing for Last-mile Logistics<br>
      <em>Advisor:</em> <a href="http://civil.iisc.ernet.in/%7Etarunr/">Prof. Tarun Rambha</a>
    </p>
  </section>

  <!-- Research Interests Section -->
  <section data-aos="fade-up">
    <h2>Research Interests</h2>
    <p>
      My primary area of interest lies in transportation network analysis, traffic assignment, and the optimization of routes with a focus on their environmental impacts. I have worked extensively on reverse logistics network design, variants of the Travelling Salesman Problem, and traffic routing. Recently, I developed a keen interest in congestion pricing and tolling.
    </p>
  </section>

  <!-- Contact Section -->
  <section data-aos="fade-up">
    <h2>Contact</h2>
    <p>
      Feel free to reach out to me via <a href="mailto:debojjalb@utexas.edu">email</a> or connect with me on <a href="https://linkedin.com/in/yourprofile">LinkedIn</a>.
    </p>
    <a href="mailto:debojjalb@utexas.edu" class="button">Email Me</a>
  </section>

  <!-- AOS Initialization -->
  <script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>
  <script>
    AOS.init();
  </script>

  <!-- Progress Bar Script -->
  <script>
    window.onscroll = function() { updateProgressBar() };

    function updateProgressBar() {
      const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
      const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
      const scrolled = (winScroll / height) * 100;
      document.getElementById("myBar").style.width = scrolled + "%";
    }
  </script>
</body>
</html>