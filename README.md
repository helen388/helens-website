<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Helen's Greek Kitchen</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #fff8f0;
      color: #333;
      line-height: 1.6;
    }

    header img {
      width: 100%;
      max-height: 300px;
      object-fit: cover;
    }

    nav {
      display: flex;
      justify-content: center;
      background-color: #e27d60;
      flex-wrap: wrap;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    nav a, nav button {
      text-decoration: none;
      color: white;
      padding: 15px 20px;
      cursor: pointer;
      font-weight: bold;
      border: none;
      background: none;
      font-size: 1em;
      transition: background 0.3s, transform 0.2s;
    }

    nav a:hover, nav button:hover {
      background-color: #c7554b;
      transform: scale(1.05);
    }

    .tab-content {
      max-width: 900px;
      margin: 20px auto;
      padding: 0 15px;
      display: none;
      animation: fadeIn 0.5s;
    }

    .tab-content.active {
      display: block;
    }

    @keyframes fadeIn {
      from {opacity:0;}
      to {opacity:1;}
    }

    .menu-item {
      margin-bottom: 25px;
      padding: 15px;
      border-left: 4px solid #e27d60;
      background-color: #fff4f0;
      border-radius: 5px;
    }

    .menu-item h3 {
      margin: 0;
      font-size: 1.2em;
      color: #e27d60;
    }

    .menu-item p {
      margin: 5px 0 0 0;
    }

    h2 {
      color: #e27d60;
      margin-top: 30px;
      border-bottom: 2px solid #e27d60;
      padding-bottom: 5px;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #e27d60;
      color: white;
      margin-top: 30px;
    }

    .order-button {
      display:inline-block;
      background-color:#e27d60;
      color:white;
      padding:12px 25px;
      border-radius:5px;
      text-decoration:none;
      font-weight:bold;
      margin-top:10px;
      transition: background 0.3s, transform 0.2s;
    }

    .order-button:hover {
      background-color: #c7554b;
      transform: scale(1.05);
    }

    @media (max-width: 600px) {
      nav a, nav button {
        padding: 10px;
        font-size: 0.9em;
      }
    }
  </style>
</head>
<body>

<header>
  <img src="banner.png" alt="Helen's Greek Kitchen Banner">
</header>

<nav>
  <a href="#about">About</a>
  <a href="#menu">Menu</a>
  <a href="#contact">Contact</a>
  <button onclick="openTab('allergens')">Allergens</button>
</nav>

<section id="about" class="tab-content active">
  <h2>About</h2>
  <p>
    Helen's Greek Kitchen – Three Cups Pub<br>
    Welcome to Helen’s Greek Kitchen at The Three Cups Pub — where the charm of a classic English pub meets the fiery heart of Greek cooking. It’s the kind of place where a hearty “OPA!” might echo over the bar, and the smell of sizzling souvlaki competes with the sound of laughter and clinking pint glasses.<br><br>

    Helen brings her passion straight from the islands — she cooks like a true Greek mama: bold flavours, no shortcuts, and a little bit of drama in every dish. From her famous moussaka and golden spanakopita to perfectly grilled souvlaki and creamy tzatziki, every bite tells a story — one that usually ends with “just one more plate.”<br><br>

    Meanwhile, The Three Cups keeps the drinks flowing — crisp pints, fine wines, and the occasional cheeky ouzo if you’re feeling brave. It’s the best of both worlds: a British pub with a Greek soul.<br><br>

    Whether you’re here for a quiet pint, a lively dinner, or to argue over who makes the best baklava, you’ll always find good food, good company, and a warm welcome — sometimes very warm, especially if Helen’s near the grill.<br><br>

    So come on in, grab a drink, and let Helen feed you like family. Because here at Helen’s Greek Kitchen at The Three Cups Pub, we don’t just serve meals — we serve moments, laughter, and a little bit of Mediterranean magic.<br><br>

    <strong>Order from 15:00 to 22:00</strong><br>
    Greek + Mediterranean + Hot food<br>
    Collection + Table orders<br>
    Order from Table QR Code
  </p>
  <a href="https://goodeats.io/helensgreek" class="order-button" target="_blank">Order Now</a>
</section>

<section id="menu" class="tab-content">
  <h2>STARTERS FOR THE GODS</h2>
  <div class="menu-item">
    <h3>Allitis Pitta</h3>
    <p>A homemade Classic from our own Greek Legend Helen. Beef Mince Meat on a pitta bread, served with a little salad and Authentic Greek Yogurt.</p>
  </div>
  <div class="menu-item">
    <h3>Feta Pastry with Honey</h3>
    <p>Crispy, Salty, Sweet and scandalously addictive. PDO Feta cheese wrapped in filo pastry and drizzled with honey & sesame.</p>
  </div>
  <div class="menu-item">
    <h3>Kolokithokeftedes</h3>
    <p>Crispy Courgettes fritters bursting with herb and Feta – Zeus himself declared them "dangerously moreish".</p>
  </div>
  <div class="menu-item">
    <h3>Greek Salad</h3>
    <p>Fresh, Crunchy and very Athenian-approved. Authentic Greek Salad with fresh tomatoes, cucumber, bell pepper, onions, olives, extra virgin olive-oil and oregano.</p>
  </div>

  <h2>WRAPS FOR THE GODS (PITA GYROS)</h2>
  <div class="menu-item">
    <h3>Pork Gyros</h3>
    <p>Juicy, smoky, and 100% approved by the intellectual Athenians. Served with fries, tomatoes, onions, and Tzatziki.</p>
  </div>
  <div class="menu-item">
    <h3>Chicken Gyros</h3>
    <p>Tastes like a Greek summer, desired by ancient Spartan warriors. Served with fries, tomatoes, onions, and Tzatziki.</p>
  </div>

  <h2>SWEET TREATS</h2>
  <div class="menu-item">
    <h3>Baklavas</h3>
    <p>Flaky, nutty, sticky perfection. Athena would swap her owl for a piece.</p>
  </div>
  <div class="menu-item">
    <h3>Chocolate Cake</h3>
    <p>Decadent, rich, and dangerously delicious. Even Hades would sneak a slice.</p>
  </div>
  <div class="menu-item">
    <h3>Orange Cake</h3>
    <p>Zesty, sweet and sun-kissed. Helios himself might approve.</p>
  </div>
  <div class="menu-item">
    <h3>Ravani</h3>
    <p>Greek semolina cake drenched in syrup. A sweet hug from the Mediterranean.</p>
  </div>
</section>

<section id="contact" class="tab-content">
  <h2>Contact</h2>
  <p>Email: info@helenskitchen.uk</p>
  <p>Phone: +44 123 456 789</p>
  <p>Address: 123 Greek Street, London, UK</p>
</section>

<section id="allergens" class="tab-content">
  <h2>Allergens</h2>
  <p>Kalos orisate! (Welcome!) At Helen's Greek Kitchen, we prepare our food with love - using traditional Greek ingredients and family recipes. We want all our guests to enjoy their meal safely, so please let us know if you have any food allergies or dietary requirements.</p>
  <p>Our dishes may contain or come into contact with the following common allergens: dairy (milk, cheese, yoghurt), gluten (wheat, barley, bread, pita, pastry), nuts (especially almonds, walnuts, pistachios), shellfish (prawns, mussels, calamari), eggs, sesame (tahini, seeds, bread toppings), soy, mustard and sulphites (found in some dressings and wines).</p>
  <p>We take great care to avoid cross-contamination, but as our kitchen handles all allergens, we cannot guarantee that any dish is completely allergen-free. Please talk to one of our lovely team members - we're always happy to help you choose something safe and delicious! Efharisto! (Thank you)</p>
</section>

<footer>
  <p>© Helen's Greek Kitchen. All rights reserved.</p>
</footer>

<script>
  function openTab(tabId) {
    const tabs = document.querySelectorAll('.tab-content');
    tabs.forEach(tab => tab.classList.remove('active'));
    document.getElementById(tabId).classList.add('active');
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }

  document.querySelectorAll('nav a').forEach(anchor => {
    anchor.addEventListener('click', function(e){
      e.preventDefault();
      const target = document.querySelector(this.getAttribute('href'));
      if(target){
        const tabs = document.querySelectorAll('.tab-content');
        tabs.forEach(tab => tab.classList.remove('active'));
        target.classList.add('active');
        window.scrollTo({ top: 0, behavior: 'smooth' });
      }
    });
  });
</script>

</body>
</html>
