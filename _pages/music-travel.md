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
  
  /* Carousel styles */
  .modal {
      display: none;
      position: fixed;
      z-index: 1000;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.8);
      overflow: auto;
  }
  .modal-content {
      position: relative;
      margin: auto;
      padding: 0;
      width: 80%;
      max-width: 700px;
  }
  .modal img {
      width: 100%;
      height: auto;
  }
  .close {
      position: absolute;
      top: 10px;
      right: 25px;
      color: #fff;
      font-size: 35px;
      font-weight: bold;
      cursor: pointer;
  }
  .carousel-controls {
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: absolute;
      top: 50%;
      width: 100%;
      transform: translateY(-50%);
  }
  .carousel-controls span {
      color: #fff;
      font-size: 30px;
      cursor: pointer;
      padding: 0 20px;
  }
</style>

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
        <td>Texas</td>
        <td><a href="#" onclick="openGallery(['texas1.jpg', 'texas2.jpg', 'texas3.jpg'])">View Photos</a></td>
      </tr>
      <tr>
        <td>Idaho</td>
        <td><a href="#" onclick="openGallery(['idaho1.jpg', 'idaho2.jpg'])">View Photos</a></td>
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
</script>
