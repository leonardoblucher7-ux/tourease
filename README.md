<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>TourEase | Travel Made Easy</title>
  <style>
    :root {
      --primary: #0ea5e9;
      --dark: #0f172a;
      --light: #f8fafc;
      --muted: #64748b;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      color: var(--dark);
      background: var(--light);
      line-height: 1.6;
    }
    header {
      background: linear-gradient(rgba(0,0,0,.45), rgba(0,0,0,.45)),
        url('https://images.unsplash.com/photo-1500530855697-b586d89ba3ee') center/cover no-repeat;
      color: white;
      padding: 80px 20px;
      text-align: center;
    }
    header h1 { font-size: 3rem; margin-bottom: 10px; }
    nav {
      display: flex;
      justify-content: center;
      gap: 20px;
      background: white;
      padding: 12px;
      position: sticky;
      top: 0;
      box-shadow: 0 2px 6px rgba(0,0,0,.08);
    }
    nav a {
      text-decoration: none;
      color: var(--dark);
      font-weight: bold;
    }
    nav a:hover { color: var(--primary); }
    section {
      padding: 60px 20px;
      max-width: 1100px;
      margin: auto;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background: white;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 8px 20px rgba(0,0,0,.08);
    }
    .card img { width: 100%; height: 180px; object-fit: cover; }
    .card div { padding: 16px; }
    .btn {
      display: inline-block;
      margin-top: 10px;
      padding: 10px 16px;
      background: var(--primary);
      color: white;
      text-decoration: none;
      border-radius: 8px;
    }
    form {
      max-width: 500px;
      margin: auto;
      background: white;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 8px 20px rgba(0,0,0,.08);
    }
    input, textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 6px;
      border: 1px solid #ccc;
      font-size: 1rem;
    }
    footer {
      background: var(--dark);
      color: white;
      text-align: center;
      padding: 30px 20px;
    }
  </style>
</head>
<body>

<header>
  <h1>TourEase</h1>
  <p>Travel Made Easy — Explore with Confidence</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#destinations">Destinations</a>
  <a href="#services">Services</a>
  <a href="#contact">Contact</a>
</nav>

<section id="home">
  <h2>Welcome to TourEase</h2>
  <p>
    TourEase helps travelers discover exciting destinations, plan trips, and travel smarter.
    Whether you're exploring locally or internationally, we make travel simple and enjoyable.
  </p>
</section>

<section id="destinations">
  <h2>Top Destinations</h2>
  <div class="grid">
    <div class="card">
      <img src="https://images.unsplash.com/photo-1505761671935-60b3a7427bad" alt="Paris">
      <div>
        <h3>Paris</h3>
        <p>Art, fashion, history, and romance in one city.</p>
      </div>
    </div>
    <div class="card">
      <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e" alt="Maldives">
      <div>
        <h3>Maldives</h3>
        <p>Relax in paradise with crystal-clear waters.</p>
      </div>
    </div>
    <div class="card">
      <img src="https://images.unsplash.com/photo-1548013146-72479768bada" alt="New York">
      <div>
        <h3>New York</h3>
        <p>Experience culture, food, and city life.</p>
      </div>
    </div>
  </div>
</section>

<section id="services">
  <h2>Our Services</h2>
  <ul>
    <li>Trip planning & itineraries</li>
    <li>Budget travel guidance</li>
    <li>Destination recommendations</li>
    <li>Travel safety tips</li>
  </ul>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <form>
    <input type="text" placeholder="Your Name" required />
    <input type="email" placeholder="Your Email" required />
    <textarea rows="5" placeholder="Your Message" required></textarea>
    <button class="btn" type="submit">Send Message</button>
  </form>
</section>

<footer>
  <p>© 2026 TourEase | Explore More, Stress Less ✈️</p>
</footer>

</body>
</html>
