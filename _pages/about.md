---
permalink: /
title: "Live with Why Not, and Think with Why"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

In retrospect, this simple principle was behind most of the 'dots' in my life that led to the most rewarding outcomes. (I find this [Steve Jobs' speech](https://youtu.be/Hd_ptbiPoXM?si=R-wkhwK40lNmLYIz&t=450) especially inspiring.)

So I am going to try to live by this principle as I’m happy with where it's led me so far.

Hi, welcome to my webpage! I am a PhD student at Purdue University in the School of Aeronautics and Astronautics. I am advised by Dr. Tanaka at the [Networked Control Systems Lab](https://networked-control-systems-lab.github.io/).

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
  
  .close-button:hover {
    color: #ccc;
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
  <figure class="gallery-item" data-image="images/cowboy.jpeg" data-caption="Dressed up as a cowboy (exchange student days)">
    <div class="thumbnail-container">
      <img src="images/cowboy.jpeg" alt="Photo 1" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Dressed up as a cowboy</figcaption>
  </figure>

  <figure class="gallery-item" data-image="images/football_torney.jpg" data-caption="First American football experience">
    <div class="thumbnail-container">
      <img src="images/football_torney.jpg" alt="Photo 2" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">First American football</figcaption>
  </figure>
  
  <figure class="gallery-item" data-image="images/hs_football.jpeg" data-caption="A local newspaper photographed me doing the iconic Heisman pose during the game">
    <div class="thumbnail-container">
      <img src="images/hs_football.jpeg" alt="Photo 3" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">The Heisman pose captured by media</figcaption>
  </figure>
  
  <figure class="gallery-item" data-image="images/natural_independence.jpeg" data-caption="The Oath of Allegiance on Independence Day">
    <div class="thumbnail-container">
      <img src="images/natural_independence.jpeg" alt="Photo 4" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Officially becoming American</figcaption>
  </figure>

  <figure class="gallery-item" data-image="images/train_army.jpeg" data-caption="Weapons training as a soldier in the US Army">
    <div class="thumbnail-container">
      <img src="images/train_army.jpeg" alt="Photo 5" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Field training</figcaption>
  </figure>

  <figure class="gallery-item" data-image="images/camo.jpeg" data-caption="Can you find me? Training with camouflage when I was in the US Army">
    <div class="thumbnail-container">
      <img src="images/camo.jpeg" alt="Photo 6" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Training camouflaged</figcaption>
  </figure>

  <figure class="gallery-item" data-image="images/skydiving.jpeg" data-caption="Jumped from an airplane at 10,000 feet">
    <div class="thumbnail-container">
      <img src="images/skydiving.jpeg" alt="Photo 7" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Skydiving</figcaption>
  </figure>

  <figure class="gallery-item" data-image="images/soccer_torney.jpeg" data-caption="Led my Korean student soccer team to tournament victory as team captain">
    <div class="thumbnail-container">
      <img src="images/soccer_torney.jpeg" alt="Photo 8" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Winning soccer tourney as a captain</figcaption>
  </figure>

  <figure class="gallery-item" data-image="images/tennis_nadal.jpeg" data-caption="Played tennis on a red clay court">
    <div class="thumbnail-container">
      <img src="images/tennis_nadal.jpeg" alt="Photo 9" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Playing tennis on a clay court</figcaption>
  </figure>

  <figure class="gallery-item" data-image="images/biking_on_campus.jpeg" data-caption="The freedom and joy of cycling across campus is a small bit of happiness">
    <div class="thumbnail-container">
      <img src="images/biking_on_campus.jpeg" alt="Photo 10" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Foldable bike</figcaption>
  </figure>

  <figure class="gallery-item" data-image="images/surfing.jpeg" data-caption="Tried surfing for the first time">
    <div class="thumbnail-container">
      <img src="images/surfing.jpeg" alt="Photo 11" class="thumbnail">
    </div>
    <figcaption class="thumbnail-caption">Surfing</figcaption>
  </figure>
</div>

<!-- Lightbox Container -->
<div id="lightbox" class="lightbox">
  <span class="close-button">&times;</span>
  <div class="lightbox-content">
    <img id="lightbox-image" class="lightbox-image" src="" alt="Enlarged photo">
    <div id="lightbox-caption" class="lightbox-caption"></div>
    <div class="lightbox-nav">
      <button class="nav-button prev-button">&lt; Previous</button>
      <button class="nav-button next-button">Next &gt;</button>
    </div>
    <div class="keyboard-hint">You can navigate through this album using arrow keys.</div>
  </div>
</div>

<!-- JavaScript for Lightbox Functionality -->
<script>
  document.addEventListener('DOMContentLoaded', function() {
    // Get all gallery items
    const galleryItems = document.querySelectorAll('.gallery-item');
    const lightbox = document.getElementById('lightbox');
    const lightboxImage = document.getElementById('lightbox-image');
    const lightboxCaption = document.getElementById('lightbox-caption');
    const closeButton = document.querySelector('.close-button');
    const prevButton = document.querySelector('.prev-button');
    const nextButton = document.querySelector('.next-button');
    
    let currentImageIndex = 0;
    let galleryImages = [];
    
    // Build the gallery images array from the actual DOM elements
    galleryItems.forEach(item => {
      galleryImages.push({
        src: item.getAttribute('data-image'),
        caption: item.getAttribute('data-caption')
      });
      
      // Add click event listener to each gallery item
      item.addEventListener('click', function() {
        const imageSrc = this.getAttribute('data-image');
        const caption = this.getAttribute('data-caption');
        
        // Find the index of the clicked image
        currentImageIndex = galleryImages.findIndex(img => img.src === imageSrc);
        
        lightboxImage.src = imageSrc;
        lightboxCaption.textContent = caption;
        lightbox.style.display = 'flex';
      });
    });
    
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
      lightboxImage.src = galleryImages[currentImageIndex].src;
      lightboxCaption.textContent = galleryImages[currentImageIndex].caption;
    }
    
    // Close lightbox
    function closeLightbox() {
      lightbox.style.display = 'none';
    }
    
    // Add event listeners for navigation and closing
    prevButton.addEventListener('click', prevImage);
    nextButton.addEventListener('click', nextImage);
    closeButton.addEventListener('click', closeLightbox);
    lightbox.addEventListener('click', function(e) {
      if (e.target === lightbox) {
        closeLightbox();
      }
    });
    
    // Keyboard navigation
    document.addEventListener('keydown', function(event) {
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
  });
</script>