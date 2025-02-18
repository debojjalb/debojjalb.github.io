---
permalink: /
title: "👋🏼 Hello there, I'm Debojjal (Deb)!"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!-- Load AOS for Animations -->
<link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
<script src="https://unpkg.com/aos@next/dist/aos.js"></script>

<style>
    /* Smooth scrolling effect */
    html {
        scroll-behavior: smooth;
    }

    /* Fade-in effect for sections */
    .fade-in {
        opacity: 0;
        transform: translateY(20px);
        transition: opacity 0.8s ease-out, transform 0.8s ease-out;
    }
    .fade-in.visible {
        opacity: 1;
        transform: translateY(0);
    }

    /* Parallax background effect */
    .parallax {
        background-image: url('your-background-image.jpg'); /* Change this */
        height: 300px;
        background-attachment: fixed;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }

    /* Typewriter effect */
    .typewriter h1 {
        overflow: hidden;
        white-space: nowrap;
        border-right: 3px solid #014552;
        animation: typing 3s steps(30, end), blink-caret 0.5s step-end infinite;
    }

    @keyframes typing {
        from { width: 0 }
        to { width: 100% }
    }

    @keyframes blink-caret {
        from, to { border-color: transparent }
        50% { border-color: #014552; }
    }
</style>

<!-- Hero Section with Typewriter Effect -->
<div class="typewriter">
    <h1>👋🏼 Hello there, I'm Debojjal (Deb)!</h1>
</div>

<!-- Parallax Background Section -->
<div class="parallax"></div>

<div class="fade-in">
    Hi! I'm currently a graduate student specializing in <a href="https://www.caee.utexas.edu/research/research-areas/transportation-engineering">Transportation Engineering</a> at the <a href="https://www.caee.utexas.edu/">University of Texas at Austin</a>. My academic journey began with a <a href="https://ug.iisc.ac.in/">BS (research)</a> degree from the <a href="https://iisc.ac.in/">Indian Institute of Science (IISc), Bangalore</a>.
</div>

<!-- Additional Content with Animations -->
<div class="fade-in">
    <h2>Education</h2>
    <p>**Master of Science in Engineering (M.S.E)** - Aug 2023 -- Fall, 2024 (Expected)</p>
</div>

<div class="fade-in">
    <h2>Research Interests</h2>
    <p>My primary area of interest lies in transportation network analysis, traffic assignment, and the optimization of routes.</p>
</div>

<div class="fade-in">
    <h2>Achievements</h2>
    <p>NTSE National Scholar, KVPY Research Fellow, MITACS Globalink Research Internship Award, Graduate School Fellowship.</p>
</div>

<div class="fade-in">
    <h2>Non Academic Interests</h2>
    <p>I am currently learning to play the guitar, enjoy chess, and love exploring new content for my YouTube channel.</p>
</div>

<!-- Initialize AOS Animations -->
<script>
    AOS.init();

    // Fade-in effect on scroll
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
</script>
