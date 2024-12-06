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
  .modal {
      display: none;
      position: fixed;
      z-index: 10000;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.8);
  }
  .modal-content {
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 90%;
      max-width: 600px;
      background: white;
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
  }
  .modal img {
      max-width: 100%;
      margin: 0 auto;
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
      text-align: center;
      color: white;
      font-size: 18px;
      cursor: pointer;
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
      <tr>
        <td>Austin, Texas</td>
        <td><a href="javascript:void(0)" onclick="openGallery(['/images/Austin1.jpeg', '/images/Austin2.jpeg'])">View Photos</a></td>
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
