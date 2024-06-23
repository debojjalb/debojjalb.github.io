---
permalink: /gallery/
title: ""
author_profile: true
redirect_from: 
  - /news/
  - /News.html
  - /news.html
---

<style>
    body {
        font-family: "Times New Roman", Times, serif;
        font-size: 14px;
        color: #000;
    }
    a {
        color: #014552; /* Dark blue color for links */
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
    .news-container {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        justify-content: center;
        margin-top: 20px;
    }
    .news-card {
        background: #fff;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        overflow: hidden;
        max-width: 300px;
        margin: 10px;
        transition: transform 0.2s;
    }
    .news-card:hover {
        transform: scale(1.05);
    }
    .news-card img {
        width: 100%;
        height: 200px;
        object-fit: cover;
    }
    .news-card .content {
        padding: 20px;
    }
    .news-card .title {
        font-size: 18px;
        font-weight: bold;
        margin-bottom: 10px;
    }
    .news-card .description {
        font-size: 14px;
        color: #666;
        margin-bottom: 10px;
    }
    .news-card .link {
        font-size: 14px;
        color: #014552;
        text-decoration: none;
    }
    .news-card .link:hover {
        text-decoration: underline;
    }
</style>

<div class="news-container">
    <div class="news-card">
        <img src="/images/UT2.jpg" alt="In front of the UT Tower">
        <div class="content">
            <div class="title">I joined UT Austin as a Grad Student</div>
            <div class="description">I am starting my MS/PhD Degree at The Fariborz Maseeh Department of Civil, Architectural and Environmental Engineering in the Cockrell School of Engineering in the Transportation Engineering Field.</div>
            <a href="/images/UT2.jpg" class="link" data-lightbox="ut-austin" data-title="In front of the UT Tower">Read more</a>
        </div>
    </div>
    <div class="news-card">
        <img src="/images/KABD.jpeg" alt="UT Transportation participated in Keep Austin Beautiful Day">
        <div class="content">
            <div class="title">Keep Austin Beautiful Day '24</div>
            <div class="description">I organised a volunteering event with UT Austin chapter of ITS/ITE along with CASITE for Keep Austin Beautiful Day 2024.</div>
            <a href="/images/KABD.jpeg" class="link" data-lightbox="keep-austin-beautiful-day" data-title="UT Transportation participated in Keep Austin Beautiful Day">Read more</a>
        </div>
    </div>
    <div class="news-card">
        <img src="/images/INFORMS.jpeg" alt="Presenting at INFORMS Annual Meeting">
        <div class="content">
            <div class="title">INFORMS Annual Meeting 2023</div>
            <div class="description">I presented our work on Electric Vehicle Last Mile Logistics. See my Research page for more details.</div>
            <a href="/images/INFORMS.jpeg" class="link" data-lightbox="informs" data-title="Presenting at INFORMS Annual Meeting">Read more</a>
        </div>
    </div>
    <div class="news-card">
        <img src="/images/Grad.png" alt="Receiving Gold Medal at IISc Bangalore">
        <div class="content">
            <div class="title">IISc Convocation</div>
            <div class="description">I graduated top of my major with a gold medal from IISc Bangalore with a Bachelor of Science (Research) degree.</div>
            <a href="/images/Grad.png" class="link" data-lightbox="iisc-convocation" data-title="Receiving Gold Medal at IISc Bangalore">Read more</a>
        </div>
    </div>
    <div class="news-card">
        <img src="/images/MITACS.png" alt="First day at UQTR">
        <div class="content">
            <div class="title">MITACS Globalink Internship 2023</div>
            <div class="description">Here's a short vlog of my typical day during MITACS.</div>
            <a href="https://youtu.be/YhyQzgftU6Y?si=9H4cYrdd136VDaGd" class="link">Watch on YouTube</a>
        </div>
    </div>
</div>
