---
permalink: /
title: "👋🏼 Hello there, I'm Debojjal (Deb)!"
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
