<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
<style>
  body {
    font-family: 'Trebuchet MS', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f0f8ff;
    color: #2e9cab;
    line-height: 1.6;
    scroll-behavior: smooth;
  }

  header img {
    width: 100%;
    height: auto;
    max-height: 400px;
    object-fit: cover;
  }

  nav {
    display: flex;
    justify-content: center;
    background-color: #2e9cab;
    flex-wrap: wrap;
    position: sticky;
    top: 0;
    z-index: 1000;
  }

  nav a {
    text-decoration: none;
    color: white;
    padding: 15px 20px;
    cursor: pointer;
    font-weight: bold;
    font-size: 1em;
    transition: background 0.3s, transform 0.2s;
  }

  nav a:hover {
    background-color: #2874a6;
    transform: scale(1.05);
  }

  section {
    max-width: 1000px;
    margin: 20px auto;
    padding: 0 20px;
  }

  h2 {
    color: #2e9cab;
    margin-top: 30px;
    border-bottom: 2px solid #2e9cab;
    padding-bottom: 5px;
  }

  .menu-item {
    margin-bottom: 20px;
    padding: 15px;
    border-left: 5px solid #2e9cab;
    background-color: #e6f2ff;
    border-radius: 8px;
  }

  .menu-item h3 {
    margin: 0 0 5px 0;
    font-size: 1.3em;
    color: #2e9cab;
  }

  .menu-item p {
    margin: 0;
    color: #2e9cab;
  }

  .allergen-list {
    list-style-type: disc;
    padding-left: 20px;
    margin: 10px 0;
    color: #2e9cab;
  }

  .order-button {
    display:inline-flex;
    align-items:center;
    justify-content:center;
    background-color:#2e9cab;
    color:white;
    padding:18px 35px;
    border-radius:50px;
    text-decoration:none;
    font-weight:bold;
    font-size:1.4em;
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    transition: background 0.3s, transform 0.2s, box-shadow 0.3s;
    margin:20px;
  }

  .order-button i {
    margin-right:10px;
    font-size:1.2em;
  }

  .order-button:hover {
    background-color: #2874a6;
    transform: scale(1.08);
    box-shadow: 0 8px 20px rgba(0,0,0,0.35);
  }

  footer {
    text-align: center;
    padding: 20px;
    background-color: #1f618d;
    color: white;
    margin-top: 30px;
  }

  /* --- Overlay alapstílus minden ablakhoz --- */
  .overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(240, 248, 255, 0.98);
    overflow-y: auto;
    display: none;
    z-index: 2000;
    padding: 50px 20px;
  }

  .overlay .close-btn {
    position: fixed;
    top: 20px;
    right: 30px;
    font-size: 2em;
    cursor: pointer;
    color: #2e9cab;
  }

  @media (max-width: 600px) {
    nav a {
      padding: 10px;
      font-size: 0.9em;
    }
    header img {
      max-height: 250px;
    }
    .order-button {
      font-size:1.2em;
      padding: 15px 25px;
    }
  }
</style>
</head>
<body>

<header>
  <img src="header2.png" alt="Helen's Greek Kitchen Banner">
</header>

<!-- Navigáció -->
<nav>
  <a id="aboutBtn">About</a>
  <a id="allergensBtn">Allergens</a>
  <a id="contactBtn">Contact</a>
</nav>

<!-- Főoldal -->
<section id="home-buttons" style="text-align:center; margin-top:50px;">
  <a id="menuBtnHome" class="order-button">
    <i class="fas fa-utensils"></i> Menu
  </a>
  <a href="https://goodeats.io/helensgreek" class="order-button" target="_blank">
    <i class="fas fa-utensils"></i> Order Now
  </a>
</section>

<!-- Overlay: MENU -->
<div id="menuOverlay" class="overlay">
  <span class="close-btn" id="closeMenu">&times;</span>
  <section id="menu">
    <!-- Itt jön az összes étel (megtartva a régi menü teljes tartalmát) -->
  </section>
</div>

<!-- Overlay: ABOUT -->
<div id="aboutOverlay" class="overlay">
  <span class="close-btn" id="closeAbout">&times;</span>
  <section id="about">
    <h2>About</h2>
    <p>
      Helen's Greek Kitchen – Three Cups Pub<br>
      Welcome to Helen’s Greek Kitchen at The Three Cups Pub — where the charm of a classic English pub meets the fiery heart of Greek cooking. Helen brings her passion straight from the islands — bold flavours, no shortcuts, and a little bit of drama in every dish. From moussaka and spanakopita to perfectly grilled souvlaki and creamy tzatziki, every bite tells a story — one that usually ends with “just one more plate.”<br><br>
      The Three Cups keeps the drinks flowing — crisp pints, fine wines, and the occasional cheeky ouzo. It’s the best of both worlds: a British pub with a Greek soul.<br><br>
      Whether you’re here for a quiet pint, a lively dinner, or to argue over who makes the best baklava, you’ll always find good food, good company, and a warm welcome.<br><br>
      <strong>Order from 15:00 to 22:00</strong><br>
      Greek + Mediterranean + Hot food<br>
      Collection + Table orders<br>
      Order from Table QR Code
    </p>
  </section>
</div>

<!-- Overlay: ALLERGENS -->
<div id="allergensOverlay" class="overlay">
  <span class="close-btn" id="closeAllergens">&times;</span>
  <section id="allergens">
    <h2>Allergens</h2>
    <ul class="allergen-list">
      <li>Gluten</li>
      <li>Crustaceans</li>
      <li>Eggs</li>
      <li>Fish</li>
      <li>Peanuts</li>
      <li>Soybeans</li>
      <li>Milk</li>
      <li>Nuts</li>
      <li>Celery</li>
      <li>Mustard</li>
      <li>Sesame seeds</li>
      <li>Sulphur dioxide and sulphites</li>
      <li>Lupin</li>
      <li>Molluscs</li>
    </ul>
  </section>
</div>

<!-- Overlay: CONTACT -->
<div id="contactOverlay" class="overlay">
  <span class="close-btn" id="closeContact">&times;</span>
  <section id="contact">
    <h2>Contact</h2>
    <p>Email: helen@helenskitchen.uk</p>
    <p>Three Cups Pub, MK403JR, Bedford 45 Newnham St</p>
  </section>
</div>

<footer>
  &copy; 2025 Helen's Greek Kitchen. All rights reserved. Designed by Miska/
</footer>

<script>
  // --- MENU OVERLAY ---
  const menuBtnHome = document.getElementById('menuBtnHome');
  const menuOverlay = document.getElementById('menuOverlay');
  const closeMenu = document.getElementById('closeMenu');

  menuBtnHome.addEventListener('click', () => menuOverlay.style.display = 'block');
  closeMenu.addEventListener('click', () => menuOverlay.style.display = 'none');
  window.addEventListener('click', (e) => {
    if(e.target === menuOverlay) menuOverlay.style.display = 'none';
  });

  // --- ABOUT OVERLAY ---
  const aboutBtn = document.getElementById('aboutBtn');
  const aboutOverlay = document.getElementById('aboutOverlay');
  const closeAbout = document.getElementById('closeAbout');

  aboutBtn.addEventListener('click', () => aboutOverlay.style.display = 'block');
  closeAbout.addEventListener('click', () => aboutOverlay.style.display = 'none');
  window.addEventListener('click', (e) => {
    if(e.target === aboutOverlay) aboutOverlay.style.display = 'none';
  });

  // --- ALLERGENS OVERLAY ---
  const allergensBtn = document.getElementById('allergensBtn');
  const allergensOverlay = document.getElementById('allergensOverlay');
  const closeAllergens = document.getElementById('closeAllergens');

  allergensBtn.addEventListener('click', () => allergensOverlay.style.display = 'block');
  closeAllergens.addEventListener('click', () => allergensOverlay.style.display = 'none');
  window.addEventListener('click', (e) => {
    if(e.target === allergensOverlay) allergensOverlay.style.display = 'none';
  });

  // --- CONTACT OVERLAY ---
  const contactBtn = document.getElementById('contactBtn');
  const contactOverlay = document.getElementById('contactOverlay');
  const closeContact = document.getElementById('closeContact');

  contactBtn.addEventListener('click', () => contactOverlay.style.display = 'block');
  closeContact.addEventListener('click', () => contactOverlay.style.display = 'none');
  window.addEventListener('click', (e) => {
    if(e.target === contactOverlay) contactOverlay.style.display = 'none';
  });
</script>

</body>
</html>
