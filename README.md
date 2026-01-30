<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>TourEase | Travel Made Easy</title>
  <style>
    :root {
      --primary: #0ea5e9;
      --secondary: #22c55e;
      --dark: #0f172a;
      --light: #f8fafc;
      --muted: #64748b;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: var(--dark);
      background: var(--light);
      line-height: 1.6;
    }
    header {
      background: linear-gradient(rgba(0,0,0,.45), rgba(0,0,0,.45)),
        url('https://images.unsplash.com/photo-1500530855697-b586d89ba3ee') center/cover no-repeat;
      color: white;
      padding: 100px 20px;
      text-align: center;
    }
    header h1 { font-size: 3.2rem; margin-bottom: 10px; }
    header p { font-size: 1.3rem; }
    nav {
      display: flex;
      justify-content: center;
      gap: 22px;
      background: white;
      padding: 14px;
      position: sticky;
      top: 0;
      z-index: 10;
      box-shadow: 0 2px 8px rgba(0,0,0,.08);
    }
    nav a {
      text-decoration: none;
      color: var(--dark);
      font-weight: bold;
    }
    nav a:hover { color: var(--primary); }
    section {
      padding: 70px 20px;
      max-width: 1150px;
      margin: auto;
    }
    .hero-stats {
      display: flex;
      justify-content: center;
      gap: 40px;
      margin-top: 30px;
      flex-wrap: wrap;
    }
    .stat {
      text-align: center;
      color: white;
    }
    .stat h3 { font-size: 2rem; margin: 0; }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 24px;
    }
    .card {
      background: white;
      border-radius: 14px;
      overflow: hidden;
      box-shadow: 0 10px 25px rgba(0,0,0,.1);
      transition: transform .3s;
    }
    .card:hover { transform: translateY(-6px); }
    .card img { width: 100%; height: 200px; object-fit: cover; }
    .card div { padding: 18px; }
    .btn {
      display: inline-block;
      margin-top: 14px;
      padding: 12px 18px;
      background: var(--primary);
      color: white;
      text-decoration: none;
      border-radius: 10px;
      font-weight: bold;
    }
    .btn.alt { background: var(--secondary); }
    .gallery img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      border-radius: 14px;
    }
    .about-box {
      background: white;
      padding: 40px;
      border-radius: 16px;
      box-shadow: 0 10px 25px rgba(0,0,0,.08);
    }
    .testimonials {
      background: #e0f2fe;
      border-radius: 16px;
      padding: 40px;
    }
    .quote { font-style: italic; }
    form {
      max-width: 520px;
      margin: auto;
      background: white;
      padding: 34px;
      border-radius: 16px;
      box-shadow: 0 10px 25px rgba(0,0,0,.1);
    }
    input, textarea {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 1rem;
    }
    footer {
      background: var(--dark);
      color: white;
      text-align: center;
      padding: 40px 20px;
    }
  </style>
</head>
<body>

<header>
  <h1>TourEase</h1>
  <p>Explore More. Stress Less. Travel Made Easy.</p>
  <div class="hero-stats">
    <div class="stat"><h3>120+</h3><p>Destinations</p></div>
    <div class="stat"><h3>10k+</h3><p>Happy Travelers</p></div>
    <div class="stat"><h3>24/7</h3><p>Support</p></div>
  </div>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#destinations">Destinations</a>
  <a href="#gallery">Gallery</a>
  <a href="#about">About</a>
  <a href="#contact">Contact</a>
</nav>

<section id="home">
  <h2>Welcome to TourEase ✈️</h2>
  <p>
    TourEase is your go-to travel companion, designed to help you plan unforgettable journeys with ease.
    From tropical beaches to bustling cities, we bring the world closer to you.
  </p>
  <a class="btn" href="#destinations">Start Exploring</a>
</section>

<section id="destinations">
  <h2>Featured Destinations</h2>
  <div class="grid">
    <div class="card">
      <img src="https://images.unsplash.com/photo-1505761671935-60b3a7427bad" alt="Paris">
      <div>
        <h3>Paris, France</h3>
        <p>Culture, fashion, art, and romance in the City of Light.</p>
      </div>
    </div>
    <div class="card">
      <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e" alt="Maldives">
      <div>
        <h3>Maldives</h3>
        <p>Turquoise waters, white sands, and total relaxation.</p>
      </div>
    </div>
    <div class="card">
      <img src="https://images.unsplash.com/photo-1548013146-72479768bada" alt="New York">
      <div>
        <h3>New York, USA</h3>
        <p>Food, culture, entertainment, and iconic skylines.</p>
      </div>
    </div>
    <div class="card">
      <img src="https://images.unsplash.com/photo-1526778548025-fa2f459cd5c1" alt="Tokyo">
      <div>
        <h3>Tokyo, Japan</h3>
        <p>Tradition meets technology in a vibrant city.</p>
      </div>
    </div>
  </div>
</section>

<section id="gallery">
  <h2>Travel Gallery</h2>
  <div class="grid gallery">
    <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470" alt="Mountains">
    <img src="https://images.unsplash.com/photo-1500534314209-a25ddb2bd429" alt="Beach">
    <img src="https://images.unsplash.com/photo-1491553895911-0055eca6402d" alt="City">
    <img src="https://images.unsplash.com/photo-1469474968028-56623f02e42e" alt="Nature">
  </div>
</section>

<section id="about">
  <h2>About TourEase</h2>
  <div class="about-box">
    <p>
      TourEase was created to make travel planning simple, exciting, and stress-free.
      Our mission is to inspire people to explore the world while providing reliable guidance,
      smart tips, and unforgettable destination ideas.
    </p>
    <p>
      Whether you're a first-time traveler or a seasoned explorer, TourEase helps you travel
      with confidence and ease.
    </p>
  </div>
</section>

<section>
  <h2>What Travelers Say</h2>
  <div class="testimonials">
    <p class="quote">“TourEase made planning my trip super easy and fun!”</p>
    <p>— Happy Traveler</p>
  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <form>
    <input type="text" placeholder="Your Name" required />
    <input type="email" placeholder="Your Email" required />
    <textarea rows="5" placeholder="Your Message" required></textarea>
    <button class="btn alt" type="submit">Send Message</button>
  </form>
</section>

<footer>
  <p>© 2026 TourEase | Explore More, Stress Less ✈️</p>
</footer>

</body>
</html>
