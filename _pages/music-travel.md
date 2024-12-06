---
permalink: /music-travel/
title: "Music and Travel Gallery"
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
  .state-map img {
      width: 100%;
      max-width: 500px;
      margin: auto;
      display: block;
  }
  .map-caption {
      text-align: center;
      font-style: italic;
      color: #666;
      margin-top: 10px;
  }
  .image-group {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
  }
  .image-group img {
      width: 200px;
      height: 150px;
      object-fit: cover;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }
</style>

<div class="section music-section">
  <h2>🎵 Music</h2>
  <p>Music is my escape. I love playing guitar and keyboard.</p>
  <p>Links to some of my guitar covers:</p>
  <ul>
    <li>Recently, my girlfriend visited me in Austin, and we recorded a cover of <a href="https://youtu.be/i9sKbcSbjF4">Purano Sei Diner Kotha</a>.</li>
    <li>This song is perfect to be played on acoustic guitar, and I believe it will be a timeless classic. Here's my version of <a href="/videos/IshqWalaLove.mov">Ishq Wala Love (इश्क वाला लव)</a>.</li>
    <li>One of my favorite licks is the opening intro to Choo Lo. <a href="/videos/Video-374.mov">Here’s my attempt! (छू लो)</a></li>
    <li>Bengali is my mother tongue, and though I never learned singing, I gave <a href="https://youtube.com/shorts/_3zst7uvgE8?si=JbpdwBvnh7QRhbRP">Coffee House er Shei Adda Ta (কফি হাউসের সেই আড্ডাটা)</a> a try.</li>
  </ul>
  <p>When back home in Kolkata, I play on my keyboard:</p>
  <ul>
    <li><a href="https://youtu.be/boWtt-A6qTU?si=vzbv0Mmv89o3w9Pc">Bosonto Eshe Geche (বসন্ত এসে গেছে)</a></li>
    <li><a href="https://youtu.be/uqbLpiiSf9M?si=j1hw4WHTiQ6bVB4t">Purano Sei Diner Kotha (পুরানো সেই দিনের কথা)</a></li>
    <li><a href="https://youtu.be/M9QqOV-6YJo?si=dbRzfBskeRMM-rgm">Pran Chay Chokhu Na Chay (প্রাণ চায় চক্ষু না চায়)</a></li>
  </ul>
</div>


<div class="section travel-section">
  <h2>✈️ Travel</h2>
  <p>I enjoy exploring new places. Click on a state to see a gallery of my travel pictures from that region.</p>
  <div class="state-map">
    <img src="/images/usa-map.png" alt="Clickable USA Map" usemap="#usamap" />
    <map name="usamap">
      <area shape="poly" coords="100,200,150,250,200,200" alt="Texas" href="/gallery/texas" />
      <area shape="poly" coords="250,300,300,350,350,300" alt="California" href="/gallery/california" />
      <!-- Add more <area> elements for each state with respective href links -->
    </map>
    <p class="map-caption">Interactive map: Click on a state to explore!</p>
  </div>
</div>

---
<!-- 
### Example Gallery Pages

**Texas Gallery:**
Create a separate page for Texas with the following structure:

```html
---
permalink: /gallery/texas/
title: "Texas Travel Gallery"
author_profile: true
---

<div class="image-group">
  <div>
    <a href="/images/texas1.jpg" data-lightbox="texas" data-title="Texas Road Trip">
      <img src="/images/texas1.jpg" alt="Texas Road Trip">
    </a>
  </div>
  <div>
    <a href="/images/texas2.jpg" data-lightbox="texas" data-title="Sunset in Austin">
      <img src="/images/texas2.jpg" alt="Sunset in Austin">
    </a>
  </div>
</div> -->
