<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>SharnTech Computer Services</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: url('https://images.unsplash.com/photo-1506748686214-e9df14d4d9d0?auto=format&fit=crop&w=1950&q=80') no-repeat center center fixed;
      background-size: cover;
      color: white;
    }

    header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 15px 30px;
      background-color: rgba(0, 0, 0, 0.8);
      position: fixed;
      top: 0;
      left: 0;
      right: 200px;
      z-index: 1000;
    }

    .logo {
      display: flex;
      align-items: center;
    }

    .logo-circle {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      background-color: #00aaff;
      color: white;
      font-weight: bold;
      font-size: 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-right: 10px;
    }

    .logo i {
      margin-left: 5px;
      font-size: 18px;
      color: white;
    }

    nav {
      position: fixed;
      top: 0;
      right: 0;
      width: 200px;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.85);
      padding-top: 100px;
    }

    nav a {
      display: block;
      color: white;
      padding: 14px 20px;
      text-decoration: none;
      font-weight: bold;
      text-align: right;
    }

    nav a:hover {
      background-color: #575757;
    }

    .content {
      margin-right: 220px;
      margin-top: 100px;
      padding: 40px;
      display: none;
    }

    .active-tab {
      display: block;
    }

    .marquee {
      font-size: 18px;
      font-weight: bold;
      margin-bottom: 20px;
      animation: colorChange 3s infinite;
    }

    @keyframes colorChange {
      0% { color: green; }
      33% { color: blue; }
      66% { color: red; }
      100% { color: green; }
    }

    .footer {
      background-color: rgba(0, 0, 0, 0.9);
      color: #ccc;
      text-align: center;
      font-size: 0.9em;
      padding: 10px;
      position: fixed;
      bottom: 0;
      left: 0;
      right: 200px;
    }

    .footer-disclaimer {
      background-color: rgba(0, 0, 0, 0.95);
      color: red;
      font-size: 0.85em;
      padding-top: 10px;
    }

    .whatsapp-btn {
      display: inline-block;
      background-color: #25d366;
      color: white;
      padding: 10px 20px;
      margin-top: 20px;
      border-radius: 5px;
      text-decoration: none;
      font-weight: bold;
    }

    .whatsapp-btn:hover {
      background-color: #1ebe5d;
    }

    ul {
      list-style: none;
      padding: 0;
    }

    ul li::before {
      content: "• ";
      color: #00ffcc;
    }

    @media screen and (max-width: 768px) {
      nav, header, .content {
        margin-right: 0;
        padding: 20px;
      }
      nav {
        position: static;
        width: 100%;
        text-align: center;
      }
      header {
        right: 0;
      }
      .footer {
        right: 0;
      }
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="logo">
      <div class="logo-circle">STC</div>
      <i class="fas fa-wifi"></i>
    </div>
  </header>

  <!-- Right Navigation -->
  <nav>
    <a href="#" onclick="showTab('home')">Home</a>
    <a href="#" onclick="showTab('about')">About</a>
    <a href="#" onclick="showTab('services')">Services</a>
    <a href="#" onclick="showTab('contact')">Contact</a>
  </nav>

  <!-- Home Section -->
  <div id="home" class="content active-tab">
    <div class="marquee">SharnTech we offer the best computer services</div>
    <h1>Welcome to SharnTech</h1>
    <p>
      Welcome to SharnTech Computer Services, your trusted partner for professional computer-related solutions.
      We are proudly based in <strong>Kitui Teachers College</strong>, and we are a <strong>legit and approved</strong>
      service provider within the institution. We offer quality, reliability, and professionalism to all students and staff.
    </p>
  </div>

  <!-- About Section -->
  <div id="about" class="content">
    <h2>About Us</h2>
    <p>
      At SharnTech, we are committed to offering the best and most reliable computer services.
      Our team is skilled in delivering practical and professional solutions. We maintain integrity and customer trust in every task we handle.
    </p>
  </div>

  <!-- Services Section -->
  <div id="services" class="content">
    <h2>Our Services</h2>
    <ul>
      <li>Word Document Typing</li>
      <li>Mobile Software Repair</li>
      <li>Laptop Software Repair</li>
      <li>Website Generation</li>
      <li>Video Editing</li>
      <li>Photo Editing</li>
      <li>Other computer-related tasks</li>
    </ul>
  </div>

  <!-- Contact Section -->
  <div id="contact" class="content">
    <h2>Contact Us</h2>
    <p><i class="fab fa-whatsapp"></i> WhatsApp: 0757614484</p>
    <p><i class="fab fa-tiktok"></i> TikTok: kenyan_flex</p>
    <p><i class="fas fa-envelope"></i> Email: stevohshark1@gmail.com</p>
    <p><i class="fab fa-facebook"></i> Facebook: Sharn flex</p>
    <p><i class="fab fa-instagram"></i> Instagram: Kenyan_flex</p>

    <a class="whatsapp-btn" target="_blank" href="https://wa.me/254757614484?text=Hello%20SharnTech%2C%20I%20would%20like%20to%20inquire%20about%20your%20services">
      <i class="fab fa-whatsapp"></i> Message Me on WhatsApp
    </a>

    <div class="footer-disclaimer">
      <p><i class="fas fa-exclamation-triangle"></i> Disclaimer:</p>
      <p>We are not running illegal business. We do not go beyond school rules and regulations!! <strong>WE DO NOT DO UNETHICAL HACKING.</strong></p>
    </div>
  </div>

  <!-- Footer on All Pages -->
  <div class="footer">
    <p>&copy; SharnTech. All rights reserved.</p>
  </div>

  <!-- Tab Script -->
  <script>
    function showTab(tabId) {
      const tabs = document.querySelectorAll('.content');
      tabs.forEach(tab => tab.classList.remove('active-tab'));
      document.getElementById(tabId).classList.add('active-tab');
    }
  </script>

</body>
</html>
