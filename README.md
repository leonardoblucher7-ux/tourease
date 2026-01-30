<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>TourEase | Book Smarter. Travel Happier.</title>
  <style>
    :root{
      --primary:#0ea5e9;
      --secondary:#22c55e;
      --accent:#f97316;
      --dark:#0f172a;
      --light:#f8fafc;
      --card:#ffffff;
      --muted:#64748b;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:'Segoe UI',Tahoma,Verdana,sans-serif;background:var(--light);color:var(--dark)}
    a{text-decoration:none;color:inherit}

    /* HEADER */
    header{
      background:linear-gradient(120deg,rgba(14,165,233,.85),rgba(34,197,94,.85)),
      url('https://images.unsplash.com/photo-1500530855697-b586d89ba3ee') center/cover no-repeat;
      color:#fff;padding:90px 20px 120px;text-align:center
    }
    header h1{font-size:3.4rem;margin:0}
    header p{font-size:1.3rem;margin:10px 0 30px}

    /* NAV */
    nav{position:sticky;top:0;z-index:20;background:#fff;display:flex;justify-content:center;gap:24px;padding:14px;box-shadow:0 2px 10px rgba(0,0,0,.08)}
    nav a{font-weight:700}
    nav a:hover{color:var(--primary)}

    /* SEARCH BOX */
    .search-wrap{max-width:1100px;margin:-70px auto 0;padding:0 20px}
    .search{
      background:#fff;border-radius:20px;box-shadow:0 20px 40px rgba(0,0,0,.15);
      padding:28px
    }
    .search h2{text-align:left;margin:0 0 16px}
    .search-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:14px}
    .search input,.search select{padding:14px;border-radius:10px;border:1px solid #d1d5db;font-size:1rem}
    .search button{
      background:var(--accent);color:#fff;border:none;border-radius:12px;
      padding:16px;font-weight:800;font-size:1rem;cursor:pointer
    }
    .search small{display:block;margin-top:10px;color:var(--muted)}

    section{max-width:1150px;margin:auto;padding:80px 20px}

    /* TRUST BAR */
    .trust{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:18px;text-align:center}
    .trust div{background:var(--card);padding:22px;border-radius:16px;box-shadow:0 10px 25px rgba(0,0,0,.08)}
    .trust h3{margin:0;font-size:1.4rem;color:var(--primary)}

    /* DEALS */
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:24px}
    .card{background:var(--card);border-radius:18px;overflow:hidden;box-shadow:0 15px 30px rgba(0,0,0,.1);transition:.3s}
    .card:hover{transform:translateY(-8px)}
    .card img{width:100%;height:200px;object-fit:cover}
    .card div{padding:18px}
    .price{color:var(--secondary);font-size:1.4rem;font-weight:800}

    /* GALLERY */
    .gallery img{width:100%;height:220px;object-fit:cover;border-radius:18px}

    /* ABOUT */
    .about{background:#e0f2fe;border-radius:22px;padding:50px;box-shadow:0 15px 30px rgba(0,0,0,.1)}

    /* TESTIMONIALS */
    .testimonial{background:#fff;border-radius:18px;padding:28px;box-shadow:0 12px 24px rgba(0,0,0,.08)}

    /* CONTACT */
    form{max-width:520px;margin:auto;background:#fff;padding:36px;border-radius:20px;box-shadow:0 15px 30px rgba(0,0,0,.12)}
    input,textarea{width:100%;padding:14px;margin:10px 0;border-radius:10px;border:1px solid #d1d5db}
    .btn{background:var(--primary);color:#fff;border:none;border-radius:12px;padding:14px 18px;font-weight:800;cursor:pointer}

    footer{background:var(--dark);color:#fff;text-align:center;padding:40px 20px}
  </style>
</head>
<body>

<header>
  <h1>TourEase</h1>
  <p>Book Smarter. Travel Happier. ✈️🌍</p>
</header>

<nav>
  <a href="#book">Flights</a>
  <a href="#deals">Deals</a>
  <a href="#gallery">Explore</a>
  <a href="#about">About</a>
  <a href="#contact">Contact</a>
</nav>

<!-- BOOKING SEARCH -->
<div class="search-wrap" id="book">
  <div class="search">
    <h2>Find Cheap Flights</h2>
    <div class="search-grid">
      <input type="text" placeholder="From (City or Airport)" />
      <input type="text" placeholder="To (City or Airport)" />
      <input type="date" />
      <input type="date" />
      <select>
        <option>1 Traveler</option><option>2 Travelers</option><option>3 Travelers</option>
      </select>
      <button>Search Flights</button>
    </div>
    <small>Compare prices from hundreds of airlines worldwide.</small>
  </div>
</div>

<section>
  <div class="trust">
    <div><h3>500+</h3><p>Airlines</p></div>
    <div><h3>Best Prices</h3><p>Guaranteed</p></div>
    <div><h3>24/7</h3><p>Customer Support</p></div>
  </div>
</section>

<section id="deals">
  <h2>🔥 Hot Flight Deals</h2>
  <div class="grid">
    <div class="card"><img src="https://images.unsplash.com/photo-1505761671935-60b3a7427bad"><div><h3>New York → Paris</h3><p class="price">From $399</p></div></div>
    <div class="card"><img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e"><div><h3>London → Maldives</h3><p class="price">From $699</p></div></div>
    <div class="card"><img src="https://images.unsplash.com/photo-1526778548025-fa2f459cd5c1"><div><h3>Los Angeles → Tokyo</h3><p class="price">From $549</p></div></div>
  </div>
</section>

<section id="gallery">
  <h2>Explore the World</h2>
  <div class="grid gallery">
    <img src="https://images.unsplash.com/photo-1501785888041-af3ef285b470">
    <img src="https://images.unsplash.com/photo-1491553895911-0055eca6402d">
    <img src="https://images.unsplash.com/photo-1469474968028-56623f02e42e">
    <img src="https://images.unsplash.com/photo-1500534314209-a25ddb2bd429">
  </div>
</section>

<section id="about">
  <h2>About TourEase</h2>
  <div class="about">
    <p><strong>TourEase</strong> is a modern travel platform built to help travelers find affordable flights, exciting destinations, and stress‑free journeys.</p>
    <p>Inspired by top booking platforms, TourEase combines smart search tools with a fun, lively experience so planning your trip feels just as exciting as taking it.</p>
  </div>
</section>

<section>
  <h2>What Travelers Say</h2>
  <div class="grid">
    <div class="testimonial"><p>“I found a cheaper flight in minutes. TourEase is a game changer!”</p><strong>— Alex</strong></div>
    <div class="testimonial"><p>“Easy, fast, and beautiful to use.”</p><strong>— Maya</strong></div>
  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <form>
    <input type="text" placeholder="Your Name" required />
    <input type="email" placeholder="Your Email" required />
    <textarea rows="5" placeholder="Your Message" required></textarea>
    <button class="btn">Send Message</button>
  </form>
</section>

<footer>
  <p>© 2026 TourEase | Book Smarter. Travel Happier ✈️</p>
</footer>

</body>
</html>
