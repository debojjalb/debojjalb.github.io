---
permalink: /music/
author_profile: true
---

<style>
  body {
      font-family: "Arial", sans-serif;
      font-size: 14px;
      color: #333;
  }
  a {
      color: #014552;
  }
  h2 {
      text-align: center;
      font-weight: bold;
      margin-top: 20px;
      margin-bottom: 20px;
  }
  a:hover {
      text-decoration: underline;
  }
  .section {
      padding: 20px;
      margin-bottom: 30px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }
  .music-section {
      background: #fdf4f7;
  }
  .travel-section {
      background: #f7faff;
  }
  table {
      margin: 20px auto;
      border-collapse: collapse;
      width: 80%;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }
  table th, table td {
      border: 1px solid #ddd;
      padding: 10px;
      text-align: center;
  }
  table th {
      background-color: #f2f2f2;
      font-weight: bold;
  }
  table a {
      text-decoration: none;
      color: #014552;
  }
  table a:hover {
      text-decoration: underline;
  }
  
  /* Modal styles */
    /* Modal styles */
    .modal {
        display: none;
        position: fixed;
        z-index: 10000; /* Higher z-index to ensure it appears above the menu */
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.8);
        overflow: hidden; /* Prevent background scrolling */
    }

    .modal-content {
        position: fixed;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        margin: 0;
        padding: 20px; /* Adds some space inside the modal */
        width: 90%; /* Use a percentage for better responsiveness */
        max-width: 600px; /* Limit the maximum width */
        max-height: 80%; /* Prevent it from overflowing the viewport */
        background: white;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        z-index: 1100; /* Ensures the content is above the modal backdrop */
        overflow: auto; /* Add scrolling for content if necessary */
    }

    .modal img {
        max-width: 100%; /* Ensure image doesn't overflow the modal */
        max-height: 100%; /* Limit the image height */
        margin: 0 auto; /* Center the image */
        display: block;
    }

    .close {
        position: absolute;
        top: 10px;
        right: 10px;
        background: rgba(0, 0, 0, 0.6);
        border-radius: 50%;
        width: 30px;
        height: 30px;
        line-height: 30px;
        text-align: center;
        color: white;
        font-size: 18px;
        font-weight: bold;
        cursor: pointer;
        transition: background 0.3s;
    }

    .carousel-controls {
        display: flex;
        justify-content: space-between;
        align-items: center;
        position: absolute;
        top: 50%;
        width: 100%;
        transform: translateY(-50%);
        z-index: 10002; /* Higher z-index to stay above the modal content */
        pointer-events: none; /* Prevent blocking clicks outside the modal */
    }

    .carousel-controls span {
        pointer-events: all; /* Enable clicking on the buttons */
        color: #fff;
        font-size: 25px;
        cursor: pointer;
        padding: 0 15px;
        background: rgba(0, 0, 0, 0.5);
        border-radius: 50%;
        width: 35px;
        height: 35px;
        line-height: 35px;
        text-align: center;
        user-select: none;
        transition: background 0.3s ease;
    }

    .carousel-controls span:hover {
        background: rgba(0, 0, 0, 0.8);
    }


</style>

<div class="section music-section">
  <h2>🎵 Music</h2>
  <p>Music is my escape. I love playing guitar and keyboard.</p>
  <p>Links to some of my guitar covers:</p>
  <ul>
    <li>Recently, my girlfriend visited me in Austin, and we recorded a cover of <a href="https://youtu.be/i9sKbcSbjF4">Purano Sei Diner Kotha (পুরানো সেই দিনের কথা)</a>.</li>
    <li>This song is perfect to be played on acoustic guitar, and I believe it will be a timeless classic. Here's my version of <a href="/videos/IshqWalaLove.mov">Ishq Wala Love (इश्क वाला लव)</a>.</li>
    <li>One of my favorite licks is the opening intro to Choo Lo. <a href="/videos/Video-374.mov">Here’s my attempt! (छू लो)</a></li>
    <!-- <li>Bengali is my mother tongue, and though I never learned singing, I gave <a href="https://youtube.com/shorts/_3zst7uvgE8?si=JbpdwBvnh7QRhbRP">Coffee House er Shei Adda Ta (কফি হাউসের সেই আড্ডাটা)</a> a try.</li> -->
  </ul>
  <p>When back home in Kolkata, I play on my keyboard:</p>
  <ul>
    <li><a href="https://youtu.be/boWtt-A6qTU?si=vzbv0Mmv89o3w9Pc">Bosonto Eshe Geche (বসন্ত এসে গেছে)</a></li>
    <li><a href="https://youtu.be/uqbLpiiSf9M?si=j1hw4WHTiQ6bVB4t">Purano Sei Diner Kotha (পুরানো সেই দিনের কথা)</a></li>
    <li><a href="https://youtu.be/M9QqOV-6YJo?si=dbRzfBskeRMM-rgm">Pran Chay Chokhu Na Chay (প্রাণ চায় চক্ষু না চায়)</a></li>
  </ul>
</div>

<<div class="section travel-section">
  <h2>🌍 Travel</h2>
  <p>Traveling lets me explore and experience new cultures, cuisines, and places. Below are some Pinterest boards that capture the beauty of different places across the world that hold special memories for me.</p>
  
  <div class="travel-columns">
    <!-- Washington -->
    <div class="travel-column">
      <h3>Washington, US</h3>
      <p>Seattle</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/washington/">
      </a>
    </div>

    <!-- Texas -->
    <div class="travel-column">
      <h3>Texas, US</h3>
      <p>Austin, San Antonio, Dallas</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/texas/">
      </a>
    </div>

    <!-- Illinois -->
    <div class="travel-column">
      <h3>Illinois, US</h3>
      <p>Chicago</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/illinois/">
      </a>
    </div>

    <!-- Quebec -->
    <div class="travel-column">
      <h3>Quebec, Canada</h3>
      <p>Montreal, Quebec City, Trois Rivieres</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/quebec/">
      </a>
    </div>

    <!-- Ontario -->
    <div class="travel-column">
      <h3>Ontario, Canada</h3>
      <p>Toronto, Niagara Falls</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/ontario/">
      </a>
    </div>

    <!-- Ottawa -->
    <div class="travel-column">
      <h3>Ottawa, Canada</h3>
      <p>Gatineau</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/ottawa/">
      </a>
    </div>

    <!-- Jaipur -->
    <div class="travel-column">
      <h3>Rajasthan, India</h3>
      <p>Jaipur</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/rajasthan/">
      </a>
    </div>

    <!-- Karnataka -->
    <div class="travel-column">
      <h3>Karnataka, India</h3>
      <p>Bangalore</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/karnataka/">
      </a>
    </div>

    <!-- Goa -->
    <div class="travel-column">
      <h3>Goa, India</h3>
      <p>Madgaon, Panjim, Vasco Da Gama</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/goa/">
      </a>
    </div>

    <!-- Indiana -->
    <div class="travel-column">
      <h3>Indiana, US</h3>
      <p>Indianapolis</p>
      <a 
          data-pin-do="embedBoard" 
          data-pin-board-width="400" 
          data-pin-scale-height="240" 
          data-pin-scale-width="60" 
          href="https://www.pinterest.com/bdebojjal/indiana/">
      </a>
    </div>
  </div>
</div>

<!-- Include Pinterest Script -->
<script async defer src="https://assets.pinterest.com/js/pinit.js"></script>

<style>
  .travel-columns {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 20px;
  }
  
  .travel-column {
      flex: 1 1 48%; /* Each column takes approximately half the width */
      box-sizing: border-box;
      padding: 10px;
      background-color: #ffffff;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }

  .travel-column h3 {
      text-align: center;
      margin-bottom: 5px;
      color: #014552;
  }

  .travel-column p {
      text-align: center;
      margin-bottom: 15px;
      font-weight: bold;
  }

  @media (max-width: 768px) {
      .travel-column {
          flex: 1 1 100%; /* Stack columns on smaller screens */
      }
  }
</style>
