---
permalink: /music-travel/
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
  
  <h3>USA</h3>
  <table>
    <thead>
      <tr>
        <th>State</th>
        <th>Gallery</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Seattle, Washington</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/INFORMS_Seattle1.jpeg', '/images/INFORMS_Seattle2.jpeg'])">View Photos</a></td>
      </tr>
      <tr>
        <td>Boise, Idaho</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/INFORMS_Seattle3.jpeg', '/images/INFORMS_Seattle4.jpeg'])">View Photos</a></td>
      </tr>
      <tr>
        <td>Chicago, Illinois</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/INFORMS_Seattle3.jpeg', '/images/INFORMS_Seattle4.jpeg'])">View Photos</a></td>
      </tr>
      <tr>
        <td>Austin, Texas</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/INFORMS_Seattle3.jpeg', '/images/INFORMS_Seattle4.jpeg'])">View Photos</a></td>
      </tr>
      <tr>
        <td>Dallas, Texas</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/INFORMS_Seattle3.jpeg', '/images/INFORMS_Seattle4.jpeg'])">View Photos</a></td>
      </tr>
      <tr>
        <td>San Antonio, Texas</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/INFORMS_Seattle3.jpeg', '/images/INFORMS_Seattle4.jpeg'])">View Photos</a></td>
      </tr>
    </tbody>
  </table>
</div>

<!-- Modal Carousel -->
<div id="galleryModal" class="modal">
  <span class="close" onclick="closeGallery()">&times;</span>
  <div class="modal-content">
    <img id="modalImage" src="" alt="Gallery Image">
    <div class="carousel-controls">
      <span id="prev" onclick="prevImage()">&#10094;</span>
      <span id="next" onclick="nextImage()">&#10095;</span>
    </div>
  </div>
</div>

<script>
  let currentImageIndex = 0;
  let images = [];

  function openGallery(imageArray) {
      images = imageArray;
      currentImageIndex = 0;
      document.getElementById('modalImage').src = images[currentImageIndex];
      document.getElementById('galleryModal').style.display = 'block';
  }

  function closeGallery() {
      document.getElementById('galleryModal').style.display = 'none';
  }

  function prevImage() {
      currentImageIndex = (currentImageIndex === 0) ? images.length - 1 : currentImageIndex - 1;
      document.getElementById('modalImage').src = images[currentImageIndex];
  }

  function nextImage() {
      currentImageIndex = (currentImageIndex === images.length - 1) ? 0 : currentImageIndex + 1;
      document.getElementById('modalImage').src = images[currentImageIndex];
  }

  document.addEventListener('click', function(event) {
      const modal = document.getElementById('galleryModal');
      if (modal.style.display === 'block' && !event.target.closest('.modal-content') && !event.target.closest('[onclick^="openGallery"]')) {
          closeGallery();
      }
  });

  document.addEventListener('keydown', function(event) {
      if (event.key === 'Escape') {
          closeGallery();
      }
  });
</script>
