<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Naveenkumar M & Pavithra C Wedding Invitation</title>

  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Sacramento&family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    * {
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: "Poppins", sans-serif;
      background: #fffaf5;
      color: #331920;
    }

    .hero {
      min-height: 100vh;
      color: #fff;
      text-align: center;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 40px 18px;
      background:
        linear-gradient(rgba(0, 0, 0, .55), rgba(0, 0, 0, .55)),
        url("Images/hero.jpg");
      background-size: cover;
      background-position: top center;
    }

    .hero h5 {
      font-size: 1rem;
      font-weight: 400;
      letter-spacing: 0;
      margin-bottom: 18px;
    }

    .hero h1 {
      font-family: "Sacramento", cursive;
      font-size: clamp(4rem, 12vw, 7rem);
      line-height: .95;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 1.05rem;
      margin-bottom: 26px;
    }

    .btn-gold {
      background: #d4af37;
      border: 0;
      color: #fff;
      font-weight: 600;
      padding: 12px 28px;
      border-radius: 999px;
      box-shadow: 0 12px 24px rgba(0, 0, 0, .22);
    }

    .btn-gold:hover,
    .btn-gold:focus {
      background: #b99323;
      color: #fff;
    }

    .section-title {
      font-family: "Sacramento", cursive;
      color: #7a0019;
      font-size: clamp(3rem, 8vw, 4.6rem);
      line-height: 1;
    }

    .cardx {
      background: #fff;
      border-radius: 8px;
      padding: 25px;
      box-shadow: 0 10px 25px rgba(0, 0, 0, .1);
      height: 100%;
    }

    .count-card {
      min-height: 120px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      gap: 6px;
    }

    .count {
      font-size: clamp(1.5rem, 5vw, 2.4rem);
      font-weight: 700;
      color: #7a0019;
      line-height: 1;
    }

    .event {
      background: linear-gradient(135deg, #7a0019, #b8860b);
      color: #fff;
      border-radius: 8px;
      padding: 30px;
    }

    .event .btn {
      border-radius: 999px;
      font-weight: 600;
    }

    .gallery-frame {
      width: min(92vw, 440px);
      margin: 28px auto 0;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: none;
      background: transparent;
      position: relative;
    }

    .gallery-track {
      display: flex;
      transition: transform .9s ease-in-out;
      will-change: transform;
    }

    .gallery-slide {
      flex: 0 0 100%;
      min-width: 100%;
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      background: transparent;
    }

    .gallery-slide img {
      width: auto;
      max-width: 100%;
      height: auto;
      max-height: 68vh;
      object-fit: contain;
      display: block;
      border-radius: 8px;
      box-shadow: 0 14px 34px rgba(0, 0, 0, .16);
    }

    .gallery-caption {
      position: absolute;
      right: 0;
      left: 0;
      bottom: 0;
      padding: 32px 20px 20px;
      background: linear-gradient(transparent, rgba(0, 0, 0, .55));
      color: #fff;
      text-align: center;
    }

    .gallery-dots {
      position: absolute;
      left: 0;
      right: 0;
      bottom: 10px;
      z-index: 3;
      display: flex;
      gap: 8px;
      justify-content: center;
      align-items: center;
    }

    .gallery-dot {
      width: 9px;
      height: 9px;
      border: 0;
      border-radius: 50%;
      background: rgba(255, 255, 255, .55);
      padding: 0;
    }

    .gallery-dot.active {
      background: #fff;
    }

    .blessing-text {
      max-width: 760px;
      margin: 0 auto;
      font-size: 1.08rem;
      line-height: 1.8;
    }

    .footer {
      background: #7a0019;
      color: #fff;
      padding: 50px 18px;
      text-align: center;
    }

    .footer h2 {
      font-family: "Sacramento", cursive;
      font-size: 3.8rem;
      margin-bottom: 12px;
    }

    .heart {
      position: fixed;
      bottom: -50px;
      font-size: 25px;
      pointer-events: none;
      z-index: 9999;
      animation: floatUp linear forwards;
      filter: drop-shadow(0 5px 6px rgba(0, 0, 0, .2));
    }

    @keyframes floatUp {
      0% {
        transform: translateY(0) scale(.5) rotate(0deg);
        opacity: 1;
      }

      100% {
        transform: translateY(-110vh) scale(1.5) rotate(20deg);
        opacity: 0;
      }
    }

    @media (max-width: 575px) {
      .hero h1 {
        font-size: 4.2rem;
      }

      .cardx {
        padding: 18px 10px;
      }
    }
  </style>
</head>

<body>
  <audio id="bgMusic" loop preload="auto">
    <source src="music.mp3" type="audio/mpeg">
  </audio>

  <section class="hero">
    <div>
      <h5>With The Blessings Of Our Families</h5>
      <h1>Naveenkumar M <br>&amp;<br>Pavithra C</h1>
      <p>25 June 2026 &bull; 4:30 AM - 6:00 AM</p>
      <button id="openBtn" class="btn btn-gold btn-lg" type="button">
        Open Invitation
      </button>
    </div>
  </section>

  <section id="invite" class="container py-5">
    <h2 class="section-title text-center">Groom &amp; Bride</h2>
    <div class="row g-4 mt-3">
      <div class="col-md-6">
        <div class="cardx text-center">
          <h3>M. Naveenkumar</h3>
          <p>Beloved Son of<br>D. Murugan &amp; Salammal</p>
        </div>
      </div>
      <div class="col-md-6">
        <div class="cardx text-center">
          <h3>C. Pavithra</h3>
          <p>Beloved Daughter of<br>Chinnaraj &amp; Nagamani</p>
        </div>
      </div>
    </div>
  </section>

  <section class="container py-5 text-center">
    <h2 class="section-title">Countdown</h2>
    <div class="row g-3 mt-4">
      <div class="col-6 col-md-3">
        <div class="cardx count-card">
          <div id="days" class="count">0</div>
          <div>Days</div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="cardx count-card">
          <div id="hours" class="count">0</div>
          <div>Hours</div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="cardx count-card">
          <div id="minutes" class="count">0</div>
          <div>Minutes</div>
        </div>
      </div>
      <div class="col-6 col-md-3">
        <div class="cardx count-card">
          <div id="seconds" class="count">0</div>
          <div>Seconds</div>
        </div>
      </div>
    </div>
  </section>

  <section class="container py-5">
    <h2 class="section-title text-center">Events</h2>

    <div class="event text-center mb-4">
      <h3>Reception</h3>
      <p>24 June 2026 &bull; 6:30 PM Onwards</p>
      <p>SSR Mandapam &amp; Marriage Hall</p>
      <a class="btn btn-warning" target="_blank" rel="noopener" href="https://maps.app.goo.gl/393FdVEkab77JVGS8">View Location</a>
    </div>

    <div class="event text-center">
      <h3>Wedding Ceremony</h3>
      <p>25 June 2026 &bull; 4:30 AM - 6:00 AM</p>
      <p>SSR Mandapam &amp; Marriage Hall</p>
      <a class="btn btn-warning" target="_blank" rel="noopener" href="https://maps.app.goo.gl/393FdVEkab77JVGS8">View Location</a>
    </div>
  </section>

  <section class="container py-5">
    <h2 class="section-title text-center">Gallery</h2>

    <div id="weddingGallery" class="gallery-frame">
      <div id="galleryTrack" class="gallery-track">
        <div class="gallery-slide">
          <img src="Images/main.jpg" alt="Wedding gallery main photo">
          <div class="gallery-caption">
            <h5>Naveenkumar &amp; Pavithra</h5>
          </div>
        </div>
        <div class="gallery-slide">
          <img src="Images/slide1.jpg" alt="Wedding gallery photo 1">
          <div class="gallery-caption">
            <h5>With Love and Blessings</h5>
          </div>
        </div>
        <div class="gallery-slide">
          <img src="Images/slide2.jpg" alt="Wedding gallery photo 2">
          <div class="gallery-caption">
            <h5>Save The Date</h5>
          </div>
        </div>
        <div class="gallery-slide">
          <img src="Images/slide3.jpg" alt="Wedding gallery photo 3">
          <div class="gallery-caption">
            <h5>Join Our Celebration</h5>
          </div>
        </div>
        <div class="gallery-slide">
          <img src="Images/slide4.jpg" alt="Wedding gallery photo 4">
          <div class="gallery-caption">
            <h5>Forever Begins Here</h5>
          </div>
        </div>
      </div>

      <div id="galleryDots" class="gallery-dots" aria-label="Gallery navigation"></div>
    </div>
  </section>

  <section class="container py-5 text-center">
    <p class="blessing-text">
      With the blessings of our parents and elders, we warmly invite you to celebrate our wedding.
      Your presence and blessings will make our special day even more memorable.
    </p>
  </section>

  <footer class="footer">
    <h2>Save The Date</h2>
    <p>Naveenkumar M &hearts; Pavithra C</p>
    <p>Reception: 24 June 2026</p>
    <p>Wedding: 25 June 2026</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

  <script>
    const openBtn = document.getElementById("openBtn");
    const bgMusic = document.getElementById("bgMusic");
    const inviteSection = document.getElementById("invite");
    const weddingDate = new Date("2026-06-25T04:30:00+05:30").getTime();
    const galleryTrack = document.getElementById("galleryTrack");
    const gallerySlides = document.querySelectorAll(".gallery-slide");
    const galleryDots = document.getElementById("galleryDots");
    let galleryIndex = 0;
    let galleryTimer;

    openBtn.addEventListener("click", () => {
      bgMusic.volume = 0.5;
      bgMusic.play().catch(() => {
        openBtn.textContent = "Tap Again To Play Music";
      });

      inviteSection.scrollIntoView({
        behavior: "smooth",
        block: "start"
      });

      startHearts();
    });

    function startHearts() {
      const duration = 10000;
      const interval = setInterval(createHeart, 150);

      setTimeout(() => {
        clearInterval(interval);
      }, duration);
    }

    function createHeart() {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerHTML = "&#10084;&#65039;";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = 18 + Math.random() * 24 + "px";
      heart.style.animationDuration = 3 + Math.random() * 4 + "s";

      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 7000);
    }

    function updateCountdown() {
      const now = new Date().getTime();
      const distance = weddingDate - now;

      if (distance <= 0) {
        document.getElementById("days").textContent = "0";
        document.getElementById("hours").textContent = "0";
        document.getElementById("minutes").textContent = "0";
        document.getElementById("seconds").textContent = "0";
        return;
      }

      document.getElementById("days").textContent = Math.floor(distance / (1000 * 60 * 60 * 24));
      document.getElementById("hours").textContent = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      document.getElementById("minutes").textContent = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      document.getElementById("seconds").textContent = Math.floor((distance % (1000 * 60)) / 1000);
    }

    updateCountdown();
    setInterval(updateCountdown, 1000);

    function showGallerySlide(index) {
      galleryIndex = (index + gallerySlides.length) % gallerySlides.length;
      galleryTrack.style.transform = "translateX(-" + galleryIndex * 100 + "%)";

      document.querySelectorAll(".gallery-dot").forEach((dot, dotIndex) => {
        dot.classList.toggle("active", dotIndex === galleryIndex);
      });
    }

    function nextGallerySlide() {
      showGallerySlide(galleryIndex + 1);
    }

    gallerySlides.forEach((slide, index) => {
      const dot = document.createElement("button");
      dot.type = "button";
      dot.className = "gallery-dot";
      dot.setAttribute("aria-label", "Show photo " + (index + 1));
      dot.addEventListener("click", () => {
        showGallerySlide(index);
        clearInterval(galleryTimer);
        galleryTimer = setInterval(nextGallerySlide, 2000);
      });
      galleryDots.appendChild(dot);
    });

    showGallerySlide(0);
    galleryTimer = setInterval(nextGallerySlide, 2000);
  </script>
</body>
</html>
