---
permalink: /
# title: "👋🏼 Hello there, I'm Debojjal  (Deb)!"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Debojjal's Site</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Source+Code+Pro:wght@400;700&display=swap');

        html, body {
            margin: 0;
            padding: 0;
            height: 100%;
            scroll-snap-type: y mandatory;
            font-family: 'Source Code Pro', monospace;
            background-color: #0d1117;
            color: #c9d1d9;
            overflow: hidden;
        }

        section {
            width: 100vw;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            scroll-snap-align: start;
        }

        .section1 {
            font-size: 3rem;
            font-weight: bold;
            color: #ff79c6;
        }

        .section2, .section3, .section4, .section5 {
            padding: 20px;
        }

        a {
            color: #ff79c6;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
            color: #ff92d0;
        }

        h1, h2, h3, h4, h5, h6 {
            font-weight: 700;
            color: #e6edf3;
        }
    </style>
</head>
<body>
    <section class="section1">
        Hi there! I'm Debojjal.<br>Welcome to my site.
    </section>
    
    <section class="section2">
        <h2>About Me</h2>
        <p>I'm currently a graduate student specializing in <a href="https://www.caee.utexas.edu/research/research-areas/transportation-engineering">Transportation Engineering</a> at UT Austin...</p>
    </section>
    
    <section class="section3">
        <h2>Research Interests</h2>
        <p>Transportation Network Optimisation, Sustainable Transportation, Congestion Pricing, Traffic Equilibrium...</p>
    </section>
    
    <section class="section4">
        <h2>Achievements</h2>
        <p>NTSE National Scholar, KVPY Research Fellow, Graduate School Fellowship at UT Austin...</p>
    </section>
    
    <section class="section5">
        <h2>Non-Academic Interests</h2>
        <p>Guitar, Chess, YouTube, Startups, Travel Enthusiast...</p>
    </section>
    
    <script>
        document.addEventListener("wheel", (event) => {
            event.preventDefault();
            window.scrollBy({ top: window.innerHeight * (event.deltaY > 0 ? 1 : -1), behavior: "smooth" });
        }, { passive: false });
    </script>
</body>
</html>
