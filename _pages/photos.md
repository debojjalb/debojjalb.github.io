<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Debojjal's Travel Gallery</title>
    <style>
        /* Global Styling */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            background: #f9f9f9;
            color: #333;
        }
        header {
            background: #ff6f61;
            color: white;
            padding: 20px;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }
        header p {
            margin: 5px 0 0;
        }

        /* Filter Buttons */
        .filter-buttons {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
        }
        .filter-buttons button {
            padding: 10px 20px;
            border: none;
            border-radius: 20px;
            background: #ff6f61;
            color: white;
            font-size: 1rem;
            cursor: pointer;
            transition: background 0.3s;
        }
        .filter-buttons button:hover {
            background: #e05b50;
        }

        /* Gallery Styling */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            padding: 20px;
        }
        .gallery-item {
            position: relative;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            background: white;
        }
        .gallery-item img {
            width: 100%;
            height: auto;
            display: block;
            transition: transform 0.3s ease;
        }
        .gallery-item:hover img {
            transform: scale(1.05);
        }
        .gallery-item .caption {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: rgba(0, 0, 0, 0.6);
            color: white;
            padding: 10px;
            text-align: center;
            font-size: 1rem;
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        .gallery-item:hover .caption {
            opacity: 1;
        }

        /* Responsive Grid */
        @media (max-width: 600px) {
            .filter-buttons {
                flex-direction: column;
                gap: 10px;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>Debojjal's Travel Gallery</h1>
    <p>Discover the beauty of the world, one city at a time!</p>
</header>

<!-- Filter Buttons -->
<div class="filter-buttons">
    <button onclick="filterGallery('all')">All</button>
    <button onclick="filterGallery('texas')">Texas</button>
    <button onclick="filterGallery('idaho')">Idaho</button>
    <button onclick="filterGallery('washington')">Washington</button>
    <button onclick="filterGallery('quebec')">Quebec</button>
    <button onclick="filterGallery('ontario')">Ontario</button>
</div>

<!-- Gallery Section -->
<div class="gallery">
    <!-- Texas Photos -->
    <div class="gallery-item texas">
        <img src="texas1.jpg" alt="Texas">
        <div class="caption">Texas - Sunset in Austin</div>
    </div>
    <div class="gallery-item texas">
        <img src="texas2.jpg" alt="Texas">
        <div class="caption">Texas - Dallas Skyscrapers</div>
    </div>

    <!-- Idaho Photos -->
    <div class="gallery-item idaho">
        <img src="idaho1.jpg" alt="Idaho">
        <div class="caption">Idaho - Mountains</div>
    </div>
    <div class="gallery-item idaho">
        <img src="idaho2.jpg" alt="Idaho">
        <div class="caption">Idaho - Peaceful Lake</div>
    </div>

    <!-- Washington Photos -->
    <div class="gallery-item washington">
        <img src="washington1.jpg" alt="Washington">
        <div class="caption">Washington - Seattle Skyline</div>
    </div>
    <div class="gallery-item washington">
        <img src="washington2.jpg" alt="Washington">
        <div class="caption">Washington - Rainy Forests</div>
    </div>

    <!-- Quebec Photos -->
    <div class="gallery-item quebec">
        <img src="quebec1.jpg" alt="Quebec">
        <div class="caption">Quebec - Old Town</div>
    </div>
    <div class="gallery-item quebec">
        <img src="quebec2.jpg" alt="Quebec">
        <div class="caption">Quebec - Winter Wonderland</div>
    </div>

    <!-- Ontario Photos -->
    <div class="gallery-item ontario">
        <img src="ontario1.jpg" alt="Ontario">
        <div class="caption">Ontario - Niagara Falls</div>
    </div>
    <div class="gallery-item ontario">
        <img src="ontario2.jpg" alt="Ontario">
        <div class="caption">Ontario - Toronto Skyline</div>
    </div>
</div>

<script>
    function filterGallery(category) {
        const items = document.querySelectorAll('.gallery-item');
        items.forEach(item => {
            if (category === 'all' || item.classList.contains(category)) {
                item.style.display = 'block';
            } else {
                item.style.display = 'none';
            }
        });
    }
</script>

</body>
</html>
