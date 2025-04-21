---
permalink: /
title: "Live with Why Not, and Think with Why"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

In many of life's pivotal moments, I was unknowlingly living by a simple principle: 

  "Live with Why Not, and Think with Why."

Reflecting on it, I still believe in this principle---and I’m happy with where it's led me.

Hi, welcome to my webpage! I am a PhD student at [Purdue University](https://www.purdue.edu/) in the [School of Aeronautics and Astronautics](https://engineering.purdue.edu/AAE). I am advised by Dr. Tanaka at the [Networked Control Systems Lab](https://networked-control-systems-lab.github.io/).

My research focus is on <em>Encrypted Control</em>, a novel field that touches upon both [control theory](https://en.wikipedia.org/wiki/Control_theory) and [cryptography](https://en.wikipedia.org/wiki/Cryptography). In this research, we apply an advanced cryptographic protocol called <em>[homomorphic encryption](https://en.wikipedia.org/wiki/Homomorphic_encryption)</em> into control systems [Cyber-Physical Systems](https://www.nsf.gov/funding/opportunities/cps-cyber-physical-systems) to **enable a privacy-preserving, secure decision-making** in the networekd control systems.

This is my professional webpage as well as my personal blog.
You can check out my CV, publications, or read up on my latest blog posts.
You can also find links to all my professional outlets on the side (or on top for mobile viewers).
If you are interested in my work, or want to collaborate, please feel free to reach out!

About Me
======
Some cool moments (that were photographed) that shaped me into who I am today.

<!-- Lightbox & Gallery Styles -->
<style>
  /* Grid layout for thumbnails */
  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
    gap: 20px;
    margin-bottom: 30px;
  }
  
  /* Thumbnail container */
  .gallery-item {
    margin: 0;
    text-align: center;
    display: flex;
    flex-direction: column;
    cursor: pointer;
    position: relative;
    border: 1px solid #eee;
    border-radius: 5px;
    overflow: hidden;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    transition: transform 0.2s, box-shadow 0.2s;
  }
  
  .gallery-item:hover {
    transform: translateY(-3px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  }
  
  /* Thumbnail image container */
  .thumbnail-container {
    height: 180px;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }
  
  /* Thumbnail image */
  .thumbnail {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s;
  }
  
  .thumbnail:hover {
    transform: scale(1.05);
  }
  
  /* Caption for thumbnails */
  .thumbnail-caption {
    font-size: 14px;
    padding: 10px;
    min-height: 40px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #f9f9f9;
    border-top: 1px solid #eee;
  }
  
  /* Lightbox overlay */
  .lightbox {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.9);
    z-index: 1000;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
  
  /* Lightbox content container */
  .lightbox-content {
    max-width: 90%;
    max-height: 80%;
    text-align: center;
  }
  
  /* Lightbox image */
  .lightbox-image {
    max-width: 100%;
    max-height: 80vh;
    object-fit: contain;
    border-radius: 5px;
  }
  
  /* Lightbox caption */
  .lightbox-caption {
    color: white;
    font-size: 18px;
    padding: 15px;
    max-width: 800px;
    margin-top: 15px;
    background-color: rgba(0, 0, 0, 0.5);
    border-radius: 5px;
  }
  
  /* Close button */
  .close-button {
    position: absolute;
    top: 20px;
    right: 30px;
    font-size: 30px;
    color: white;
    cursor: pointer;
    transition: color 0.2s;
  }
  
  .lightbox-nav {
    display: flex;
    justify-content: space-between;
    width: 100%;
    max-width: 400px;
    margin-top: 20px;
  }
  
  .nav-button {
    background-color: rgba(255, 255, 255, 0.2);
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
    transition: background-color 0.2s;
  }
  
  .nav-button:hover {
    background-color: rgba(255, 255, 255, 0.3);
  }
  
  .keyboard-hint {
    color: rgba(255, 255, 255, 0.6);
    font-size: 12px;
    margin-top: 15px;
    text-align: center;
  }
</style>

<!-- Gallery Grid -->
<div class="gallery-grid">
  <figure class="gallery-item" onclick="openLightbox('/images/cowboy.jpeg', 'Dressed up as a cowboy (exchange student days)')">
    <div class="thumbnail-container">
      <img src="/images/cowboy.jpeg" alt="Photo 1" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Dressed up as a cowboy</figcaption>
  </figure>

  <figure class="gallery-item" onclick="openLightbox('/images/football_torney.jpg', 'First American football experience')">
    <div class="thumbnail-container">
      <img src="/images/football_torney.jpg" alt="Photo 2" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">First American football</figcaption>
  </figure>
  
  <figure class="gallery-item" onclick="openLightbox('/images/hs_football.jpeg', 'A local news took a cool picture of me with the Heisman pose')">
    <div class="thumbnail-container">
      <img src="/images/hs_football.jpeg" alt="Photo 3" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">A local newspaper captured me with the Heisman pose</figcaption>
  </figure>

  <figure class="gallery-item" onclick="openLightbox('/images/soccer_torney.jpeg', 'Led my Korean student soccer team to win a local tournament as a captain')">
    <div class="thumbnail-container">
      <img src="/images/soccer_torney.jpeg" alt="Photo 9" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Winning soccer tourney as a captain</figcaption>
  </figure>
  
  <figure class="gallery-item" onclick="openLightbox('/images/natural_independence.jpeg', 'The Oath of Allegiance on the Independence day')">
    <div class="thumbnail-container">
      <img src="/images/natural_independence.jpeg" alt="Photo 4" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Officially becoming American</figcaption>
  </figure>

  <figure class="gallery-item" onclick="openLightbox('/images/train_army.jpeg', 'Field training days in the US Army')">
    <div class="thumbnail-container">
      <img src="/images/train_army.jpeg" alt="Photo 5" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Field training</figcaption>
  </figure>

  <figure class="gallery-item" onclick="openLightbox('/images/camo.jpeg', 'Training with a camouflage in the field')">
    <div class="thumbnail-container">
      <img src="/images/camo.jpeg" alt="Photo 6" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Training camouflaged</figcaption>
  </figure>

  <figure class="gallery-item" onclick="openLightbox('/images/skydiving.jpeg', 'Jumped from an airplane at 10,000 feet')">
    <div class="thumbnail-container">
      <img src="/images/skydiving.jpeg" alt="Photo 7" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">First skydiving</figcaption>
  </figure>

  <figure class="gallery-item" onclick="openLightbox('/images/surfing.jpeg', 'Tried surfing for the first time')">
    <div class="thumbnail-container">
      <img src="/images/surfing.jpeg" alt="Photo 8" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">First surfing</figcaption>
  </figure>

  <figure class="gallery-item" onclick="openLightbox('/images/tennis_nadal.jpeg', 'Played tennis on a red clay court')">
    <div class="thumbnail-container">
      <img src="/images/tennis_nadal.jpeg" alt="Photo 9" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Playing tennis on a clay court</figcaption>
  </figure>

  <figure class="gallery-item" onclick="openLightbox('/images/biking_on_campus.jpeg', 'Biking on a campus is a great feeling')">
    <div class="thumbnail-container">
      <img src="/images/biking_on_campus.jpeg" alt="Photo 9" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Riding my foldable bike</figcaption>
  </figure>

</div>

<!-- Lightbox Container -->
<div id="lightbox" class="lightbox" onclick="closeLightbox()">
  <span class="close-button">&times;</span>
  <div class="lightbox-content" onclick="event.stopPropagation()">
    <img id="lightbox-image" class="lightbox-image" src="" alt="Enlarged photo">
    <div id="lightbox-caption" class="lightbox-caption"></div>
    <div class="lightbox-nav">
      <button class="nav-button prev-button" onclick="prevImage()">&lt; Previous</button>
      <button class="nav-button next-button" onclick="nextImage()">Next &gt;</button>
    </div>
    <div class="keyboard-hint">Use ← → arrow keys to navigate</div>
  </div>
</div>

<!-- JavaScript for Lightbox Functionality -->
<script>
  // Store image data for navigation
  const galleryImages = [
    { src: '/images/cowboy.jpeg', caption: 'Dressed up as a cowboy (exchange student days)' },
    { src: '/images/football_torney.jpg', caption: 'First American football experience' },
    { src: '/images/hs_football.jpeg', caption: 'A local news took a cool picture of me with the Heisman pose' },
    { src: '/images/soccer_torney.jpeg', caption: 'Led my Korean student soccer team to win a local tournament as a captain' },
    { src: '/images/natural_independence.jpeg', caption: 'The Oath of Allegiance on the Independence day' },
    { src: '/images/train_army.jpeg', caption: 'Field training days in the US Army' },
    { src: '/images/camo.jpeg', caption: 'Training with a camouflage in the field' },
    { src: '/images/skydiving.jpeg', caption: 'Jumped from an airplane at 10,000 feet' },
    { src: '/images/surfing.jpeg', caption: 'Tried surfing for the first time' },
    { src: '/images/tennis_nadal.jpeg', caption: 'Played tennis on a red clay court' },
    { src: '/images/biking_on_campus.jpeg', caption: 'Riding my foldable bike' },

  ];
  
  let currentImageIndex = 0;
  
  // Open lightbox with the clicked image
  function openLightbox(imageSrc, caption) {
    const lightbox = document.getElementById('lightbox');
    const lightboxImage = document.getElementById('lightbox-image');
    const lightboxCaption = document.getElementById('lightbox-caption');
    
    // Find the index of the clicked image
    currentImageIndex = galleryImages.findIndex(img => img.src === imageSrc);
    
    lightboxImage.src = imageSrc;
    lightboxCaption.textContent = caption;
    lightbox.style.display = 'flex';
    
    // Prevent the click from bubbling up and immediately closing
    event.stopPropagation();
  }
  
  // Navigate to previous image
  function prevImage() {
    currentImageIndex = (currentImageIndex - 1 + galleryImages.length) % galleryImages.length;
    updateLightboxImage();
  }
  
  // Navigate to next image
  function nextImage() {
    currentImageIndex = (currentImageIndex + 1) % galleryImages.length;
    updateLightboxImage();
  }
  
  // Update the lightbox with current image
  function updateLightboxImage() {
    const lightboxImage = document.getElementById('lightbox-image');
    const lightboxCaption = document.getElementById('lightbox-caption');
    
    lightboxImage.src = galleryImages[currentImageIndex].src;
    lightboxCaption.textContent = galleryImages[currentImageIndex].caption;
  }
  
  // Close lightbox
  function closeLightbox() {
    document.getElementById('lightbox').style.display = 'none';
  }
  
  // Keyboard navigation
  document.addEventListener('keydown', function(event) {
    const lightbox = document.getElementById('lightbox');
    // Only handle keyboard navigation when lightbox is open
    if (lightbox.style.display === 'flex') {
      switch(event.key) {
        case 'ArrowLeft':
          prevImage();
          event.preventDefault();
          break;
        case 'ArrowRight':
          nextImage();
          event.preventDefault();
          break;
        case 'Escape':
          closeLightbox();
          event.preventDefault();
          break;
      }
    }
  });
</script>

<!-- Lightbox Container -->
<div id="lightbox" class="lightbox" onclick="closeLightbox()">
  <span class="close-button">&times;</span>
  <div class="lightbox-content">
    <img id="lightbox-image" class="lightbox-image" src="" alt="Enlarged photo">
    <div id="lightbox-caption" class="lightbox-caption"></div>
  </div>
</div>

<!-- JavaScript for Lightbox Functionality -->
<script>
  // Open lightbox with the clicked image
  function openLightbox(imageSrc, caption) {
    const lightbox = document.getElementById('lightbox');
    const lightboxImage = document.getElementById('lightbox-image');
    const lightboxCaption = document.getElementById('lightbox-caption');
    
    lightboxImage.src = imageSrc;
    lightboxCaption.textContent = caption;
    lightbox.style.display = 'flex';
    
    // Prevent the click from bubbling up and immediately closing
    event.stopPropagation();
  }
  
  // Close lightbox
  function closeLightbox() {
    document.getElementById('lightbox').style.display = 'none';
  }
  
  // Close lightbox when ESC key is pressed
  document.addEventListener('keydown', function(event) {
    if (event.key === 'Escape') {
      closeLightbox();
    }
  });
</script>
