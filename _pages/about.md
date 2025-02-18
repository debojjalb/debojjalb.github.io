---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Debojjal's Portfolio</title>
    
    <!-- FullPage.js CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/fullPage.js/3.1.2/fullpage.min.css">

    <style>
        @import url('https://fonts.googleapis.com/css2?family=Source+Code+Pro:wght@400;700&display=swap');

        body {
            font-family: 'Source Code Pro', monospace;
            font-size: 16px;
            background-color: #0d1117;
            color: #c9d1d9;
            margin: 0;
            padding: 0;
        }

        /* Ensure each section takes up full screen */
        .section {
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        a {
            color: #58a6ff; /* GitHub blue */
            text-decoration: none;
        }
        
        a:hover {
            text-decoration: underline;
        }

        h1, h2, h3, h4, h5, h6 {
            font-weight: 700;
            color: #e6edf3;
        }

        .typing-container {
            font-size: 28px;
            font-weight: bold;
            color: #58a6ff;
            height: 50px;
            white-space: nowrap;
            overflow: hidden;
            border-right: 4px solid #58a6ff;
            width: 0;
            animation: typing 3s steps(35, end) forwards, blinkCursor 0.8s infinite;
        }
        
        @keyframes typing {
            from { width: 0; }
            to { width: 280px; }
        }

        @keyframes blinkCursor {
            50% { border-color: transparent; }
        }
    </style>
</head>
<body>

<!-- Full Page Scroll Sections -->
<div id="fullpage">
    <div class="section">
        <div class="typing-container">Hello there, I'm Debojjal (Deb)!</div>
        <p>Welcome to my personal site.</p>
    </div>

    <div class="section">
        <h2>About me</h2>
        <p>
        Hi! I'm currently a graduate student specializing in [Transportation Engineering](https://www.caee.utexas.edu/research/research-areas/transportation-engineering) at the [Department of Civil, Architectural, and Environmental Engineering](https://www.caee.utexas.edu/), [University of Texas at Austin](https://www.utexas.edu/). My academic journey began with a [BS (research)](https://ug.iisc.ac.in/) degree from the [Indian Institute of Science (IISc), Bangalore](https://iisc.ac.in/), where I majored in Earth & Environmental Science along with a minor in Mathematics. During my time there, I was associated with the [Transportation Networks Lab](http://civil.iisc.ernet.in/%7Etarunr/group.html) at the [Center for Infrastructure, Sustainable Transportation & Urban Planning (CiSTUP)](https://cistup.iisc.ac.in/). Over the past two years, I have delved into sustainable logistics and transportation.

        My roots trace back to the picturesque city of Kalyani, nestled near Kolkata. I then moved to Bangalore, often referred to as the Garden City of India, for my undergraduate studies. Currently, I call the vibrant and musically-rich city of Austin my home. 

        Thank you for visiting my site. I invite you to explore the site and learn more about my research. Should you wish to discuss my research or simply chat, please don't hesitate to reach out via [email](mailto:debojjalb@utexas.edu).
        </p>
    </div>

    <div class="section">
        <h2>Education</h2>
        <p><strong>Master of Science in Engineering (M.S.E)</strong> - UT Austin</p>
        <p><strong>Bachelor of Science (B.S.)</strong> - IISc Bangalore</p>
    </div>

    <div class="section">
        <h2>Research Interests</h2>
        <p>Transportation Network Optimization, Congestion Pricing, Sustainable Transport.</p>
    </div>

    <div class="section">
        <h2>Achievements</h2>
        <p>NTSE Scholar, KVPY Fellow, MITACS Intern, UT Austin Graduate Fellowship.</p>
    </div>

    <div class="section">
        <h2>Non-Academic Interests</h2>
        <p>Guitar, Chess, YouTube Content Creation, Travel, Startups.</p>
    </div>
</div>

<!-- FullPage.js Library -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/fullPage.js/3.1.2/fullpage.min.js"></script>
<script>
    new fullpage('#fullpage', {
        autoScrolling: true,
        navigation: true,
        navigationPosition: 'right',
        scrollHorizontally: true
    });
</script>

</body>
</html>
