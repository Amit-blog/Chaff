<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My One Page Website</title>
  <style>
    /* Basic Reset */
    * {margin: 0; padding: 0; box-sizing: border-box;}
    body {font-family: Arial, sans-serif; line-height: 1.6;}

    Navbar
    nav {
      position: fixed;
      top: 0; left: 0;
      width: 100%;
      background: #333;
      padding: 15px;
      text-align: center;
      z-index: 1000;
    }
    nav a {
      color: #fff; text-decoration: none;
      margin: 0 15px; font-weight: bold;
    }
    nav a:hover {color: #00bcd4;}

    /* Sections */
    section {
      padding: 80px 20px;
      min-height: 100vh;
    }
    #home {
      background: url('https://picsum.photos/1920/1080?blur') no-repeat center center/cover;
      color: white; display: flex;
      flex-direction: column;
      justify-content: center; align-items: center;
      text-align: center;
    }
    #home h1 {font-size: 3rem; margin-bottom: 10px;}
    #home p {font-size: 1.2rem;}

    #about {background: #f4f4f4;}
    #products {background: #fff;}
    #contact {background: #f4f4f4;}

    /* Product Cards */
    .products-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .product {
      border: 1px solid #ddd;
      border-radius: 10px;
      padding: 15px;
      text-align: center;
      background: #fff;
      transition: 0.3s;
    }
    .product:hover {box-shadow: 0 0 10px rgba(0,0,0,0.2);}
    .product img {max-width: 100%; border-radius: 10px;}

    /* Contact Form */
    form {max-width: 500px; margin: auto;}
    input, textarea {
      width: 100%; padding: 10px; margin: 10px 0;
      border: 1px solid #ccc; border-radius: 5px;
    }
    button {
      background: #00bcd4; color: white;
      padding: 10px 20px; border: none;
      border-radius: 5px; cursor: pointer;
    }
    button:hover {background: #0097a7;}

    /* Footer */
    footer {
      text-align: center;
      padding: 20px;
      background: #333; color: white;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#products">Products</a>
    <a href="#contact">Contact</a>
  </nav>

  <!-- Home -->
  <section id="home">
    <h1>Welcome to My Store</h1>
    <p>Best Products at Affordable Prices</p>
  </section>

  <!-- About -->
  <section id="about">
    <h2>About Us</h2>
    <p>We provide high-quality products made with love and care. 
    Our mission is to bring you the best shopping experience online.</p>
  </section>

  <!-- Products -->
  <section id="products">
    <h2>Our Products</h2>
    <div class="products-container">
      <div class="product">
        <img src="https://picsum.photos/300/200?1" alt="Product 1">
        <h3>Product 1</h3>
        <p>₹499</p>
        <button>Buy Now</button>
      </div>
      <div class="product">
        <img src="https://picsum.photos/300/200?2" alt="Product 2">
        <h3>Product 2</h3>
        <p>₹799</p>
        <button>Buy Now</button>
      </div>
      <div class="product">
        <img src="https://picsum.photos/300/200?3" alt="Product 3">
        <h3>Product 3</h3>
        <p>₹999</p>
        <button>Buy Now</button>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="5" placeholder="Your Message"></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 My Store | All Rights Reserved</p>
  </footer>

</body>
</html>
