---
permalink: /building/
title: "👋🏼 Hello there, I'm Debojjal (Deb)!"
author_profile: true
redirect_from: 
  - /building/
  - /building.html
---

<!-- Load AOS for Animations -->
<link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
<script src="https://unpkg.com/aos@next/dist/aos.js"></script>

<style>
    /* Smooth scrolling */
    html {
        scroll-behavior: smooth;
    }

    /* Ensure the full page is visible */
    body {
        font-family: "Arial", sans-serif;
        font-size: 16px;
        line-height: 1.6;
        color: #333;
        margin: 0;
        padding: 20px;
        background-color: #f9f9f9;
    }

    /* Typewriter effect */
    .typewriter h1 {
        overflow: hidden;
        white-space: nowrap;
        border-right: 3px solid #014552;
        animation: typing 2s steps(30, end) forwards, blink-caret 0.5s step-end infinite;
        font-size: 28px;
        color: #014552;
        text-align: center;
    }

    @keyframes typing {
        from { width: 0 }
        to { width: 100% }
    }

    @keyframes blink-caret {
        from, to { border-color: transparent }
        50% { border-color: #014552; }
    }

    /* Content fade-in effect */
    .fade-in {
        opacity: 0;
        transform: translateY(20px);
        transition: opacity 1s ease-out, transform 1s ease-out;
    }

    .fade-in.visible {
        opacity: 1;
        transform: translateY(0);
    }

    /* Parallax section */
    .parallax {
        background-image: url('https://source.unsplash.com/1600x900/?city,transport'); /* Replace with your image */
        height: 300px;
        background-attachment: fixed;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        margin-bottom: 40px;
    }

    /* Section container */
    .section {
        background: white;
        padding: 40px;
        border-radius: 10px;
        box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
        margin-bottom: 20px;
    }

</style>

<!-- Typewriter Effect -->
<div class="typewriter">
    <h1>👋🏼 Hello there, I'm Debojjal (Deb)!</h1>
</div>

<!-- Parallax Section -->
<div class="parallax"></div>

<!-- Page Content with Animations -->
<div class="fade-in section">
    <h2>About Me</h2>
    <p>Hi! I'm currently a graduate student specializing in <a href="https://www.caee.utexas.edu/research/research-areas/transportation-engineering">Transportation Engineering</a> at the <a href="https://www.caee.utexas.edu/">University of Texas at Austin</a>. My academic journey began with a <a href="https://ug.iisc.ac.in/">BS (research)</a> degree from the <a href="https://iisc.ac.in/">Indian Institute of Science (IISc), Bangalore</a>.</p>
</div>

<div class="fade-in section">
    <h2>Education</h2>
    <p><strong>Master of Science in Engineering (M.S.E)</strong> - Aug 2023 -- Fall, 2024 (Expected)</p>
</div>

<div class="fade-in section">
    <h2>Research Interests</h2>
    <p>My primary area of interest lies in transportation network analysis, traffic assignment, and the optimization of routes.</p>
</div>

<div class="fade-in section">
    <h2>Achievements</h2>
    <p>NTSE National Scholar, KVPY Research Fellow, MITACS Globalink Research Internship Award, Graduate School Fellowship.</p>
</div>

<div class="fade-in section">
    <h2>Non-Academic Interests</h2>
    <p>I am currently learning to play the guitar, enjoy chess, and love exploring new content for my YouTube channel.</p>
</div>

<!-- Initialize AOS Animations -->
<script>
    AOS.init();

    // Ensure fade-in effect works on scroll
    document.addEventListener("DOMContentLoaded", function() {
        const fadeIns = document.querySelectorAll('.fade-in');
        function revealOnScroll() {
            fadeIns.forEach((el) => {
                if (el.getBoundingClientRect().top < window.innerHeight * 0.9) {
                    el.classList.add("visible");
                }
            });
        }
        window.addEventListener("scroll", revealOnScroll);
        revealOnScroll();
    });

    // Stop blinking cursor after animation
    setTimeout(() => {
        document.querySelector('.typewriter h1').style.borderRight = "none";
    }, 2000);
</script>