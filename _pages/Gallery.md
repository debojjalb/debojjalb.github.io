---
permalink: /gallery/
title: "Gallery"
author_profile: true
redirect_from: 
  - /gal/
  - /gallery.html
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Slider</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: "Georgia", serif;
            font-size: 16px;
            color: #333;
            background-color: #f8f8f8;
            line-height: 1.6;
        }
        a {
            color: #0074D9; /* Vivid blue color for links */
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        h1, h2, h3, h4, h5, h6 {
            margin-top: 24px;
            margin-bottom: 16px;
            font-weight: 700;
            line-height: 1.25;
            color: #111;
        }
        .image-group {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 20px;
            margin-bottom: 40px;
            overflow: hidden;
            position: relative;
        }
        .image-group .slide {
            display: flex;
        }
        .image-group .slide div {
            min-width: 100%;
            transition: transform 0.5s ease;
            text-align: center;
        }
        .image-group img {
            width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .caption {
            font-style: italic;
            color: #666;
            margin-top: 8px;
        }
        .prev, .next {
            cursor: pointer;
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            border: none;
            font-size: 18px;
            border-radius: 50%;
            padding: 10px;
        }
        .prev {
            left: 10px;
        }
        .next {
            right: 10px;
        }
    </style>
</head>
<body>
    <h2>I joined UT Austin as a Grad Student</h2>
    <div class="image-group two-images">
        <div class="slide">
            <div>
                <img src="/images/UT2.jpg" alt="In front of the UT Tower">
                <p class="caption">In front of the UT Tower</p>
            </div>
            <div>
                <img src="/images/UT.jpg" alt="With friends from India in Austin">
                <p class="caption">With friends from India in Austin</p>
            </div>
        </div>
        <button class="prev">&#10094;</button>
        <button class="next">&#10095;</button>
    </div>

    <h2>IISc Convocation</h2>
    <div class="image-group three-images">
        <div class="slide">
            <div>
                <img src="/images/Grad.png" alt="Receiving Gold Medal at IISc Bangalore">
                <p class="caption">Receiving Gold Medal at IISc Bangalore</p>
            </div>
            <div>
                <img src="/images/IISc.jpg" alt="Friends from IISc '23 batch">
                <p class="caption">Friends from IISc '23 batch</p>
            </div>
            <div>
                <img src="/images/IIScGrad.jpg" alt="With parents in front of IISc Main Building">
                <p class="caption">With parents in front of IISc Main Building</p>
            </div>
        </div>
        <button class="prev">&#10094;</button>
        <button class="next">&#10095;</button>
    </div>

    <script>
        document.querySelectorAll('.image-group').forEach(function(group) {
            let slideIndex = 0;
            let slides = group.querySelectorAll('.slide div');
            let prevButton = group.querySelector('.prev');
            let nextButton = group.querySelector('.next');

            function showSlide(index) {
                if (index >= slides.length) {
                    slideIndex = 0;
                } else if (index < 0) {
                    slideIndex = slides.length - 1;
                } else {
                    slideIndex = index;
                }
                slides.forEach((slide, i) => {
                    slide.style.transform = `translateX(-${slideIndex * 100}%)`;
                });
            }

            prevButton.addEventListener('click', () => {
                showSlide(--slideIndex);
            });

            nextButton.addEventListener('click', () => {
                showSlide(++slideIndex);
            });

            showSlide(slideIndex);
        });
    </script>
</body>
</html>





<!-- ---
permalink: /gallery/
title: "Gallery"
author_profile: true
redirect_from: 
  - /gal/
  - /gallery.html
---

<style>
    body {
        font-family: "Georgia", serif;
        font-size: 16px;
        color: #333;
        background-color: #f8f8f8;
        line-height: 1.6;
    }
    a {
        color: #0074D9; /* Vivid blue color for links */
        text-decoration: none;
    }
    a:hover {
        text-decoration: underline;
    }
    h1, h2, h3, h4, h5, h6 {
        margin-top: 24px;
        margin-bottom: 16px;
        font-weight: 700;
        line-height: 1.25;
        color: #111;
    }
    .image-group {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        gap: 20px;
        margin-bottom: 40px;
    }
    .image-group div {
        flex: 1;
        text-align: center;
    }
    .image-group img {
        width: 100%;
        height: auto;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    .caption {
        font-style: italic;
        color: #666;
        margin-top: 8px;
    }
</style>

## I joined UT Austin as a Grad Student

<div class="image-group two-images">
    <div>
        <img src="/images/UT2.jpg" alt="In front of the UT Tower">
        <p class="caption">In front of the UT Tower</p>
    </div>
    <div>
        <img src="/images/UT.jpg" alt="With friends from India in Austin">
        <p class="caption">With friends from India in Austin</p>
    </div>
</div>

## IISc Convocation

<div class="image-group three-images">
    <div>
        <img src="/images/Grad.png" alt="Receiving Gold Medal at IISc Bangalore">
        <p class="caption">Receiving Gold Medal at IISc Bangalore</p>
    </div>
    <div>
        <img src="/images/IISc.jpg" alt="Friends from IISc '23 batch">
        <p class="caption">Friends from IISc '23 batch</p>
    </div>
    <div>
        <img src="/images/IIScGrad.jpg" alt="With parents in front of IISc Main Building">
        <p class="caption">With parents in front of IISc Main Building</p>
    </div>
</div>

## INFORMS Annual Meeting 2023

<div class="image-group two-images">
    <div>
        <img src="/images/INFORMS.jpeg" alt="Presenting at INFORMS Annual Meeting">
        <p class="caption">Presenting at INFORMS Annual Meeting, Indianapolis</p>
    </div>
    <div>
        <img src="/images/Chicago.jpg" alt="Detour to Chicago">
        <p class="caption">Detour to Chicago</p>
    </div>
</div>

## MITACS Globalink Internship 2023

<div class="image-group three-images">
    <div>
        <img src="/images/MITACS.png" alt="First day at UQTR">
        <p class="caption">First day at UQTR</p>
    </div>
    <div>
        <img src="/images/MITACS_Mentor.jpg" alt="With MITACS Intern and mentor">
        <p class="caption">With MITACS Intern and mentor</p>
    </div>
    <div>
        <img src="/images/MITACS4.jpg" alt="City of Trois-Rivières">
        <p class="caption">City of Trois-Rivières</p>
    </div>
</div>

## I visted Canada as a part of MITACS Globalink Internship

<div class="image-group two-images">
    <div>
        <img src="/images/Toronto.jpg" alt="View of Downtown Toronto from CN Tower">
        <p class="caption">View of Downtown Toronto from CN Tower</p>
    </div>
    <div>
        <img src="/images/Ottawa.jpg" alt="Parliament Hill and Peace Tower in Ottawa">
        <p class="caption">Parliament Hill and Peace Tower in Ottawa</p>
    </div>
</div>
<div class="image-group two-images">
    <div>
        <img src="/images/Montreal.jpg" alt="Fireworks Festival in Montreal">
        <p class="caption">Fireworks Festival in Montreal</p>
    </div>
    <div>
        <img src="/images/Quebec.jpg" alt="Downtown Quebec City">
        <p class="caption">Downtown Quebec City</p>
    </div>
</div>

## Niagara Falls

<div class="image-group three-images">
    <div>
        <img src="/images/Niagara.jpg" alt="Niagara Falls at Night">
        <p class="caption">Niagara Falls at Night</p>
    </div>
    <div>
        <img src="/images/Niagara2.jpg" alt="Boat ride into Niagara Falls">
        <p class="caption">Boat ride into Niagara Falls</p>
    </div>
    <div>
        <img src="/images/Niagara3.jpg" alt="White Water Walk near Niagara Falls">
        <p class="caption">White Water Walk near Niagara Falls</p>
    </div>
</div>


## The Telegraph School Awards

<div class="image-group one-image">
    <div>
        <img src="/images/TELEGRAPH.jpeg" alt="Father receiving Telegraph School Award">
        <p class="caption">Father receiving Telegraph School Award</p>
    </div>
</div>

## JBNSTS Award Ceremony

<div class="image-group one-image">
    <div>
        <img src="/images/JBNSTS.jpeg" alt="Receiving JBNSTS Award">
        <p class="caption">Receiving JBNSTS Award</p>
    </div>
</div> -->
