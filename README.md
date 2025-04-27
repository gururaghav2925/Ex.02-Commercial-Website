# Ex02 Commercial Website
## Date:11.03.2025
## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
# Index.html

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>BusinessPro - Commercial Website</title>
  <link rel="stylesheet" href="commercial.css">
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
</head>
<body>

  <!-- Header -->
  <header class="header">
    <div class="container nav-container">
      <div class="logo">Business<span>Pro</span></div>
      <nav>
        <ul class="nav-links">
          <li><a href="#services">Services</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero" style="background-image: url(https://imgs.search.brave.com/Bm8iIe3puMUuxIGnWMONW_GwVI3VizjE06_yGTFKr2U/rs:fit:500:0:0:0/g:ce/aHR0cHM6Ly9pLnBp/bmltZy5jb20vb3Jp/Z2luYWxzLzYxLzRh/L2ZkLzYxNGFmZDUz/ODg3YWQyZDM1ZjM0/NDg3NzljYmMyOGMz/LmpwZw) ;background-repeat: no-repeat; background-size: cover;">
    <div class="container hero-content">
      <h1>Empower Your Business With <span>BusinessPro</span></h1>
      <p>We help brands grow with tailored web solutions, digital marketing, and strategic innovation.</p>
      <a href="#contact" class="btn">Get Started</a>
    </div>
  </section>

  <!-- Services Section -->
  <section id="services" class="section services">
    <div class="container">
      <h2 class="section-title">Our Services</h2>
      <div class="services-grid">
        <div class="service-card">
          <img src="https://images.unsplash.com/photo-1542744173-05336fcc7ad4?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=60" alt="Web Development">
          <h3>Web Development</h3>
          <p>Custom websites and applications tailored to your business needs.</p>
        </div>
        <div class="service-card">
          <img src="https://imgs.search.brave.com/FqhlEAO_aO2TKlnq56Twq6MUd1B5N5wYKeBBJn9Pbc4/rs:fit:500:0:0:0/g:ce/aHR0cHM6Ly93YWxs/cGFwZXJzLmNvbS9p/bWFnZXMvaGQvZGln/aXRhbC1tYXJrZXRp/bmctcGljdHVyZXMt/dnM0ZjAzbXpzN2Zk/bnVrNi5qcGc" alt="Digital Marketing">
          <h3>Digital Marketing</h3>
          <p>Boost your brand presence with SEO, PPC, and social media strategies.</p>
        </div>
        <div class="service-card">
          <img src="https://imgs.search.brave.com/cT3btSNgIBoTcrkr1T1E5uakPyQXyTVvte05uzb4trI/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly90NC5m/dGNkbi5uZXQvanBn/LzA5Lzk5LzU1Lzk3/LzM2MF9GXzk5OTU1/OTczNF9lRVZ5ZU43/eWVWMWRyV2EwYWFK/cWkwWmtpS0JXd2pz/ei5qcGc" alt="Consulting">
          <h3>Consulting</h3>
          <p>Expert business advice to help you scale and innovate smarter.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="section about">
    <div class="container about-content">
      <div class="about-text">
        <h2>About Us</h2>
        <p>At BusinessPro, we specialize in delivering modern, scalable, and efficient digital solutions. Our mission is to empower businesses with technology and innovative strategies to achieve remarkable growth.</p>
      </div>
      <img src="https://images.unsplash.com/photo-1570129477492-45c003edd2be?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=60" alt="Team Work">
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="section contact" style="background-image: url(https://t3.ftcdn.net/jpg/05/30/96/04/360_F_530960431_c8fPd3HansYvrSJ4fJxZqp9OhjQmYoll.jpg);background-repeat: no-repeat; background-size: cover;">
    <div class="container">
      <h2 class="section-title">Contact Us</h2>
      <p>Ready to elevate your brand? Let’s talk business!</p>
      <a href="mailto:info@businesspro.com" class="btn">Email Us</a>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="container">
      <p>&copy; 2025 BusinessPro. All rights reserved.</p>
    </div>
  </footer>

</body>
</html>




```

# Index.css

````
/* Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  
  body {
    font-family: 'Poppins', sans-serif;
    color: #333;
    background: #f9f9f9;
  }
  
  .container {
    width: 90%;
    max-width: 1200px;
    margin: auto;
  }
  
  /* Header */
  .header {
    background: #0078ff;
    padding: 20px 0;
  }
  
  .nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .logo {
    font-size: 28px;
    font-weight: 700;
    color: #fff;
  }
  
  .logo span {
    color: #00d4ff;
  }
  
  .nav-links {
    list-style: none;
    display: flex;
    gap: 25px;
  }
  
  .nav-links a {
    color: #fff;
    text-decoration: none;
    font-weight: 600;
    transition: color 0.3s;
  }
  
  .nav-links a:hover {
    color: #00d4ff;
  }
  
  /* Hero */
  .hero {
    background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
      url('https://images.unsplash.com/photo-1581090700227-4c4a989e1aa5?ixlib=rb-4.0.3&auto=format&fit=crop&w=1600&q=80') no-repeat center/cover;
    color: #fff;
    text-align: center;
    padding: 160px 20px;
  }
  
  .hero h1 {
    font-size: 48px;
    margin-bottom: 20px;
  }
  
  .hero span {
    color: #00d4ff;
  }
  
  .hero p {
    font-size: 20px;
    margin-bottom: 30px;
  }
  
  .btn {
    background: #00d4ff;
    color: #fff;
    padding: 14px 32px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    transition: background 0.4s;
  }
  
  .btn:hover {
    background: #0078ff;
  }
  
  /* Sections */
  .section {
    padding: 80px 0;
    text-align: center;
  }
  
  .section-title {
    font-size: 36px;
    margin-bottom: 40px;
    color: #0078ff;
  }
  
  /* Services */
  .services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 30px;
  }
  
  .service-card {
    background: #fff;
    border-radius: 8px;
    padding: 20px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    transition: transform 0.3s;
  }
  
  .service-card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
    border-radius: 8px 8px 0 0;
  }
  
  .service-card h3 {
    margin: 20px 0 10px;
  }
  
  .service-card p {
    font-size: 15px;
    color: #555;
  }
  
  .service-card:hover {
    transform: translateY(-10px);
  }
  
  /* About */
  .about-content {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 40px;
  }
  
  .about-text {
    flex: 1;
    min-width: 280px;
    text-align: left;
  }
  
  .about-content img {
    width: 400px;
    height: auto;
    border-radius: 8px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.15);
  }
  
  /* Contact */
  .contact p {
    margin-bottom: 20px;
  }
  
  /* Footer */
  .footer {
    background: #222;
    color: #aaa;
    text-align: center;
    padding: 20px;
    font-size: 14px;
  }
  






````

## OUTPUT


![image](https://github.com/user-attachments/assets/3fcda913-84b9-4dbc-8930-7873211286a3)


![image](https://github.com/user-attachments/assets/c3c69aab-977f-4664-9e40-dc88ec3f05c4)

![image](https://github.com/user-attachments/assets/75773271-5f52-482e-a5c0-72fb12bf6d63)


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
