---
permalink: /travel/
author_profile: true
---


<style>
  body {
      font-family: "Arial", sans-serif;
      font-size: 14px;
      color: #333;
  }
  h2 {
      text-align: center;
      font-weight: bold;
      margin: 20px 0;
  }
  table {
      margin: 20px auto;
      border-collapse: collapse;
      width: 80%;
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

  /* Modal styles */
  .modal {
      display: none;
      position: fixed;
      z-index: 10000;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.9);
      overflow: hidden;
  }
  .modal.show {
      display: block;
      overflow: hidden;
  }
  body.modal-open {
      overflow: hidden; /* Disable scrolling */
  }
  .modal-content {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      max-width: 90%;
      max-height: 80%;
      text-align: center;
  }
  .modal-content img {
      width: 100%;
      height: auto;
      border-radius: 10px;
  }
  .thumbnails {
      display: flex;
      justify-content: center;
      margin-top: 20px;
  }
  .thumbnails img {
      width: 80px;
      height: 60px;
      margin: 0 5px;
      cursor: pointer;
      border: 2px solid transparent;
      border-radius: 5px;
      transition: transform 0.2s ease-in-out, border 0.2s ease-in-out;
  }
  .thumbnails img:hover,
  .thumbnails img.active {
      transform: scale(1.1);
      border: 2px solid white;
  }
  .carousel-controls {
      position: absolute;
      width: 100%;
      top: 50%;
      transform: translateY(-50%);
      display: flex;
      justify-content: space-between;
  }
  .carousel-controls span {
      cursor: pointer;
      color: white;
      font-size: 40px;
      padding: 10px;
      background: rgba(0, 0, 0, 0.5);
      border-radius: 50%;
      user-select: none;
  }
  .close {
      position: absolute;
      top: 20px;
      right: 20px;
      color: white;
      font-size: 40px;
      cursor: pointer;
      background: rgba(0, 0, 0, 0.6);
      border-radius: 50%;
      text-align: center;
      width: 40px;
      height: 40px;
      line-height: 40px;
      user-select: none;
  }
</style>

<div class="section travel-section">
  <h2>✈️ Travel</h2>
  <p>Click on a state to see a gallery of my travel pictures from that region.</p>

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
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/Seattle1.jpeg', '/images/Seattle2.jpeg'])">View Photos</a></td>
      </tr>
      <tr>
        <td>Boise, Idaho</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/Boise1.jpeg', '/images/Boise2.jpeg'])">View Photos</a></td>
      </tr>
      <tr>
        <td>Chicago, Illinois</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/Chicago1.jpeg', '/images/Chicago2.jpeg'])">View Photos</a></td>
      </tr>
    </tbody>
  </table>
</div>

<div id="galleryModal" class="modal">
  <span class="close" onclick="closeGallery()">&times;</span>
  <div class="modal-content">
    <img id="modalImage" src="" alt="Gallery Image">
    <div class="carousel-controls">
      <span id="prev" onclick="prevImage()">&#10094;</span>
      <span id="next" onclick="nextImage()">&#10095;</span>
    </div>
    <div class="thumbnails" id="thumbnails"></div>
  </div>
</div>

<script>
  let currentImageIndex = 0;
  let images = [];

  function openGallery(imageArray) {
      images = imageArray;
      currentImageIndex = 0;
      updateGallery();
      document.body.classList.add('modal-open'); // Disable scrolling
      document.getElementById('galleryModal').classList.add('show');
  }

  function closeGallery() {
      document.getElementById('galleryModal').classList.remove('show');
      document.body.classList.remove('modal-open'); // Enable scrolling
  }

  function prevImage() {
      currentImageIndex = (currentImageIndex === 0) ? images.length - 1 : currentImageIndex - 1;
      updateGallery();
  }

  function nextImage() {
      currentImageIndex = (currentImageIndex === images.length - 1) ? 0 : currentImageIndex + 1;
      updateGallery();
  }

  function updateGallery() {
      document.getElementById('modalImage').src = images[currentImageIndex];
      const thumbnailsDiv = document.getElementById('thumbnails');
      thumbnailsDiv.innerHTML = images.map((src, index) => 
          `<img src="${src}" class="${index === currentImageIndex ? 'active' : ''}" onclick="setImage(${index})">`
      ).join('');
  }

  function setImage(index) {
      currentImageIndex = index;
      updateGallery();
  }
</script>
