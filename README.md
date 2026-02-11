<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Portfolio | Presentation Designer</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }

    body {
      background: #fafafa;
      color: #1f2933;
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    .container {
      max-width: 1100px;
      margin: auto;
      padding: 40px 20px;
    }

    /* Header */
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 80px;
    }

    .logo {
      font-weight: 700;
      font-size: 22px;
    }

    nav a {
      margin-left: 25px;
      font-size: 15px;
      color: #555;
    }

    nav a:hover {
      color: #000;
    }

    .lang-switch {
      margin-left: 25px;
      cursor: pointer;
      font-size: 14px;
      color: #111;
      font-weight: 600;
    }

    /* Hero */
    .hero {
      max-width: 700px;
      margin-bottom: 100px;
    }

    .hero h1 {
      font-size: 48px;
      font-weight: 700;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: 18px;
      color: #555;
      margin-bottom: 30px;
    }

    .btn {
      display: inline-block;
      padding: 12px 26px;
      background: #111;
      color: #fff;
      border-radius: 6px;
      font-size: 15px;
      transition: 0.3s;
    }

    .btn:hover {
      background: #333;
    }

    section {
      margin-bottom: 100px;
    }

    section h2 {
      font-size: 32px;
      margin-bottom: 40px;
      font-weight: 600;
    }

    /* Portfolio */
    .portfolio-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
    }

    .card {
      background: #fff;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 5px 15px rgba(0,0,0,0.05);
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }

    .card-content {
      padding: 20px;
    }

    .card-content h3 {
      margin-bottom: 8px;
      font-size: 18px;
    }

    .card-content p {
      font-size: 14px;
      color: #666;
    }

    /* About */
    .about {
      max-width: 700px;
    }

    .about p {
      font-size: 17px;
      color: #444;
    }

    /* Contact */
    .contact-box {
      background: #fff;
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.05);
      max-width: 600px;
    }

    .contact-box p {
      margin-bottom: 15px;
      font-size: 16px;
    }

    footer {
      text-align: center;
      padding: 40px 0;
      color: #777;
      font-size: 14px;
    }

    @media(max-width:768px){
      .hero h1{
        font-size:36px;
      }

      header{
        flex-direction:column;
        gap:15px;
      }
    }
  </style>
</head>
<body>

  <div class="container">

    <!-- Header -->
    <header>
      <div class="logo">Rifaldi.</div>
      <nav>
        <a href="#home" data-id="navHome">Home</a>
        <a href="#portfolio" data-id="navPortfolio">Portfolio</a>
        <a href="#about" data-id="navAbout">About</a>
        <a href="#contact" data-id="navContact">Contact</a>
        <span class="lang-switch" onclick="toggleLang()" id="langBtn">EN</span>
      </nav>
    </header>

    <!-- Hero -->
    <section class="hero" id="home">
      <h1 data-id="heroTitle">Presentation Designer & Visual Storyteller</h1>
      <p data-id="heroDesc">
        Saya membantu brand dan bisnis menyampaikan ide mereka
        melalui presentasi yang profesional, menarik, dan mudah dipahami.
      </p>
      <a href="#portfolio" class="btn" data-id="heroBtn">Lihat Portfolio</a>
    </section>

    <!-- Portfolio -->
    <section id="portfolio">
      <h2 data-id="portTitle">Portfolio</h2>

      <div class="portfolio-grid">

        <div class="card">
          <img src="https://source.unsplash.com/600x400/?presentation,office" alt="Project 1">
          <div class="card-content">
            <h3 data-id="p1Title">Pitch Deck Startup</h3>
            <p data-id="p1Desc">Desain presentasi untuk investor dan pitching.</p>
          </div>
        </div>

        <div class="card">
          <img src="https://source.unsplash.com/600x400/?business,meeting" alt="Project 2">
          <div class="card-content">
            <h3 data-id="p2Title">Company Profile</h3>
            <p data-id="p2Desc">Company profile modern untuk perusahaan.</p>
          </div>
        </div>

        <div class="card">
          <img src="https://source.unsplash.com/600x400/?work,desk,design" alt="Project 3">
          <div class="card-content">
            <h3 data-id="p3Title">Training Module</h3>
            <p data-id="p3Desc">Slide edukasi dan training internal.</p>
          </div>
        </div>

      </div>
    </section>

    <!-- About -->
    <section id="about">
      <h2 data-id="aboutTitle">About Me</h2>

      <div class="about">
        <p data-id="aboutDesc">
          Saya adalah seorang presentation designer yang fokus
          pada visual storytelling, struktur informasi, dan
          desain yang bersih. Berpengalaman membuat slide untuk
          bisnis, edukasi, dan pitching.
        </p>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact">
      <h2 data-id="contactTitle">Contact</h2>

      <div class="contact-box">
        <p><strong>Email:</strong> your@email.com</p>
        <p><strong>WhatsApp:</strong> +62xxxxxxxxxx</p>
        <p><strong>LinkedIn:</strong> linkedin.com/in/username</p>
        <a href="mailto:your@email.com" class="btn" data-id="contactBtn">Hire Me</a>
      </div>
    </section>

    <!-- Footer -->
    <footer data-id="footerText">
      © 2026 Rifaldi Darma Putra. All rights reserved.
    </footer>

  </div>

<script>
  let currentLang = "id";

  const content = {
    id: {
      navHome: "Home",
      navPortfolio: "Portfolio",
      navAbout: "Tentang",
      navContact: "Kontak",
      heroTitle: "Presentation Designer & Visual Storyteller",
      heroDesc: "Saya membantu brand dan bisnis menyampaikan ide mereka melalui presentasi yang profesional, menarik, dan mudah dipahami.",
      heroBtn: "Lihat Portfolio",
      portTitle: "Portfolio",
      p1Title: "Pitch Deck Startup",
      p1Desc: "Desain presentasi untuk investor dan pitching.",
      p2Title: "Company Profile",
      p2Desc: "Company profile modern untuk perusahaan.",
      p3Title: "Training Module",
      p3Desc: "Slide edukasi dan training internal.",
      aboutTitle: "Tentang Saya",
      aboutDesc: "Saya adalah seorang presentation designer yang fokus pada visual storytelling, struktur informasi, dan desain yang bersih. Berpengalaman membuat slide untuk bisnis, edukasi, dan pitching.",
      contactTitle: "Kontak",
      contactBtn: "Hubungi Saya",
      footerText: "© 2026 Rifaldi Darma Putra. All rights reserved."
    },
    en: {
      navHome: "Home",
      navPortfolio: "Portfolio",
      navAbout: "About",
      navContact: "Contact",
      heroTitle: "Presentation Designer & Visual Storyteller",
      heroDesc: "I help brands and businesses deliver their ideas through professional, engaging, and easy-to-understand presentations.",
      heroBtn: "View Portfolio",
      portTitle: "Portfolio",
      p1Title: "Startup Pitch Deck",
      p1Desc: "Presentation design for investors and pitching.",
      p2Title: "Company Profile",
      p2Desc: "Modern company profile presentation.",
      p3Title: "Training Module",
      p3Desc: "Educational and internal training slides.",
      aboutTitle: "About Me",
      aboutDesc: "I am a presentation designer focused on visual storytelling, information structure, and clean design. Experienced in creating slides for business, education, and pitching.",
      contactTitle: "Contact",
      contactBtn: "Hire Me",
      footerText: "© 2026 Rifaldi Darma Putra. All rights reserved."
    }
  };

  function toggleLang() {
    currentLang = currentLang === "id" ? "en" : "id";
    document.getElementById("langBtn").innerText = currentLang === "id" ? "EN" : "ID";

    document.querySelectorAll("[data-id]").forEach(el => {
      const key = el.getAttribute("data-id");
      el.innerText = content[currentLang][key];
    });

    document.documentElement.lang = currentLang;
  }
</script>

</body>
</html>
