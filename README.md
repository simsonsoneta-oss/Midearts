<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Midearts - Custom Resin Art Case</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
  <style>
    :root {
      --navy: #0b0f1a;
      --gold: #d4af37;
      --rose: #f4c2c2;
      --text: #f5f5f5;
    }

    html { scroll-behavior: smooth; }

    body {
      margin: 0;
      background-color: var(--navy);
      color: var(--text);
      font-family: "Poppins", sans-serif;
      overflow-x: hidden;
      animation: fadeIn 1.5s ease;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    nav {
      background: rgba(15,15,25,0.8);
      backdrop-filter: blur(10px);
      position: sticky;
      top: 0;
      z-index: 10;
      padding: 1rem 2rem;
    }

    nav ul { list-style: none; display: flex; justify-content: space-between; align-items: center; margin: 0; padding: 0; }
    nav a { color: var(--gold); text-decoration: none; margin: 0 1rem; transition: 0.3s; }
    nav a:hover { color: var(--rose); }

    header {
      background-image: url('https://images.unsplash.com/photo-1616627562888-1ef23a0b77ce?auto=format&fit=crop&w=1400&q=80');
      background-size: cover;
      background-attachment: fixed;
      background-position: center;
      text-align: center;
      padding: 8rem 2rem;
      position: relative;
    }

    header::after {
      content: "";
      position: absolute;
      inset: 0;
      background: rgba(0, 0, 0, 0.6);
    }

    header * { position: relative; z-index: 1; }
    header h1 { font-size: 3rem; color: var(--gold); margin-bottom: 1rem; }
    header p { font-size: 1.2rem; color: var(--rose); }

    .cta {
      background: var(--gold);
      color: var(--navy);
      border: none;
      padding: 0.8rem 2rem;
      border-radius: 6px;
      margin-top: 2rem;
      cursor: pointer;
      font-weight: bold;
      transition: all 0.3s;
    }

    .cta:hover { background: #e3bf57; }

    section {
      padding: 4rem 2rem;
      text-align: center;
      max-width: 900px;
      margin: auto;
    }

    section h2 { color: var(--gold); margin-bottom: 1rem; }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
      padding: 2rem 0;
    }

    .gallery figure {
      aspect-ratio: 1/1;
      overflow: hidden;
      border-radius: 10px;
      margin: 0;
      transition: transform 0.3s ease;
    }

    .gallery img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      transition: transform 0.4s ease;
    }

    .gallery img:hover { transform: scale(1.08); }

    footer {
      background: rgba(15,15,25,0.9);
      color: var(--rose);
      text-align: center;
      padding: 2rem 1rem;
      margin-top: 2rem;
    }

    footer a {
      color: var(--gold);
      text-decoration: none;
      margin: 0 0.5rem;
    }

    footer a:hover { color: var(--rose); }
  </style>
</head>
<body>

  <nav>
    <ul>
      <li><strong style="color: var(--gold); font-size: 1.2rem;">Midearts</strong></li>
      <li>
        <a href="#tentang">Tentang</a>
        <a href="#galeri">Galeri</a>
        <a href="#kontak">Kontak</a>
      </li>
    </ul>
  </nav>

  <header>
    <h1>Midearts</h1>
    <p>Seni, keindahan, dan keunikan dalam setiap custom resin art case handmade.</p>
    <button class="cta" onclick="document.getElementById('galeri').scrollIntoView({behavior: 'smooth'})">Lihat Katalog</button>
  </header>

  <section id="tentang">
    <h2>Tentang Kami</h2>
    <p>
      Midearts adalah brand seni resin handmade yang menghadirkan case ponsel dengan sentuhan personal dan elegan.
      Setiap karya dibuat dengan hati — menghadirkan harmoni warna, tekstur, dan kilau yang mencerminkan karakter pemiliknya.
    </p>
  </section>

  <section id="galeri">
    <h2>Katalog Produk</h2>
    <div class="gallery">
      <figure><img src="https://images.unsplash.com/photo-1606813902912-f43d11bcbf68?auto=format&fit=crop&w=800&q=80" alt="Resin Case 1"></figure>
      <figure><img src="https://images.unsplash.com/photo-1602524819929-070d60e2b3f1?auto=format&fit=crop&w=800&q=80" alt="Resin Case 2"></figure>
      <figure><img src="https://images.unsplash.com/photo-1616627562888-1ef23a0b77ce?auto=format&fit=crop&w=800&q=80" alt="Resin Case 3"></figure>
      <figure><img src="https://images.unsplash.com/photo-1606813902912-f43d11bcbf68?auto=format&fit=crop&w=800&q=80" alt="Resin Case 4"></figure>
    </div>
  </section>

  <section id="kontak">
    <h2>Hubungi Kami</h2>
    <p>Ingin custom case unik? Hubungi kami untuk konsultasi desain gratis.</p>
    <p>
      <!-- Ganti tanda pagar (#) di bawah dengan tautan kamu -->
      <a href="#" role="button" class="contrast">Instagram</a>
      <a href="#" role="button" class="secondary">WhatsApp</a>
    </p>
  </section>

  <footer>
    <small>© 2025 Midearts • <a href="#">Instagram</a> • <a href="#">WhatsApp</a></small>
  </footer>

</body>
</html>
