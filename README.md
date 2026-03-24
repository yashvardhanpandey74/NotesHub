<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NotesHUB</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      font-family: Arial, sans-serif;
      color: #fff;
    }

    /* Sidebar menu */
    .sidebar {
      width: 250px;
      background-color: rgba(0,0,0,0.8);
      padding-top: 20px;
      position: fixed;
      height: 100%;
      overflow-y: auto;
      animation: slideIn 1.5s ease forwards;
    }

    .sidebar h2 {
      text-align: center;
      margin-bottom: 20px;
      font-size: 1.8em;
      color: #00c6ff;
    }

    .sidebar a {
      display: block;
      padding: 12px 20px;
      text-decoration: none;
      color: #fff;
      transition: background 0.3s;
    }

    .sidebar a:hover {
      background-color: #203a43;
    }

    /* Dropdown for subjects */
    .dropdown {
      padding: 12px 20px;
      cursor: pointer;
      background-color: rgba(255,255,255,0.05);
    }

    .dropdown:hover {
      background-color: #203a43;
    }

    .dropdown-content {
      display: none;
      flex-direction: column;
      background-color: rgba(0,0,0,0.6);
    }

    .dropdown-content a {
      padding: 10px 40px;
      font-size: 0.95em;
    }

    .dropdown:hover .dropdown-content {
      display: flex;
    }

    /* Main content */
    .main {
      margin-left: 250px;
      flex: 1;
      padding: 20px;
      text-align: center;
    }

    .main h1 {
      font-size: 3.5em;
      margin-top: 20px;
      text-shadow: 2px 2px 8px rgba(0,0,0,0.7);
      opacity: 0;
      transform: translateY(-30px);
      animation: fadeInDown 2s ease forwards;
    }

    /* Banner section */
    .banner {
      margin-top: 30px;
      background: rgba(0, 198, 255, 0.2);
      padding: 30px;
      border-radius: 10px;
      display: inline-block;
      animation: fadeIn 2s ease forwards;
    }

    .banner h2 {
      font-size: 2em;
      margin-bottom: 10px;
      color: #00c6ff;
    }

    .banner p {
      font-size: 1.1em;
      max-width: 600px;
      margin: auto;
      line-height: 1.5;
    }

    /* FAQ section */
    .faq {
      margin-top: 40px;
      background: rgba(255, 255, 255, 0.1);
      padding: 25px;
      border-radius: 10px;
      animation: fadeIn 2s ease forwards;
    }

    .faq h2 {
      text-align: center;
      color: #00c6ff;
      margin-bottom: 20px;
      font-size: 2em;
    }

    .faq-item {
      margin-bottom: 15px;
      text-align: left;
    }

    .faq-item h3 {
      color: #00c6ff;
      font-size: 1.2em;
      margin-bottom: 5px;
    }

    .faq-item p {
      font-size: 1em;
      line-height: 1.5;
    }

    /* Animations */
    @keyframes fadeInDown {
      0% { opacity: 0; transform: translateY(-30px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes slideIn {
      from { transform: translateX(-100%); }
      to { transform: translateX(0); }
    }
  </style>
</head>
<body>
  <div class="sidebar">
    <h2>Menu</h2>
    <a href="#">About</a>
    <a href="#">Contact Us</a>
    <a href="#">Question Paper</a>
    <div class="dropdown">
      Subjects ▼
      <div class="dropdown-content">
        <a href="#">Engineering Maths 1</a>
        <a href="#">Engineering Maths 2</a>
        <a href="#">Semiconductor Physics</a>
        <a href="#">Electrical</a>
        <a href="#">Mechanical</a>
        <a href="#">Digital Electronics</a>
        <a href="#">Discrete Maths</a>
      </div>
    </div>
  </div>

  <div class="main">
    <h1>NotesHUB</h1>
    <div class="banner">
      <h2>Highest Quality Notes</h2>
      <p>
        NotesHUB provides well-structured, reliable, and easy-to-understand notes 
        across multiple subjects. Our resources are curated to help students excel 
        in academics with clarity and confidence. Thank You..!!
      </p>
    </div>

    <!-- FAQ Section -->
    <div class="faq">
      <h2>Frequently Asked Questions</h2>
      <div class="faq-item">
        <h3>What is NotesHUB?</h3>
        <p>NotesHUB is a platform that provides high-quality, easy-to-understand notes across multiple subjects to help students excel in academics.</p>
      </div>
      <div class="faq-item">
        <h3>Are the notes free?</h3>
        <p>Yes, all notes provided on NotesHUB are free to access for students.</p>
      </div>
      <div class="faq-item">
        <h3>How often are notes updated?</h3>
        <p>We regularly update our notes to ensure accuracy and relevance with the latest syllabus and exam patterns.</p>
      </div>
      <div class="faq-item">
        <h3>Can I request notes for a specific subject?</h3>
        <p>Absolutely! You can contact us through the "Contact Us" section to request notes for subjects not yet listed.</p>
      </div>
    </div>
  </div>
</body>
</html>
