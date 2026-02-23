# Ex02 Commercial Website
## Date:23.02.2026

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
Index.html
```
<!DOCTYPE html>
<html>
<head>
  <title>Simple E-Commerce</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      scroll-behavior: smooth;
      background: #f4f4f4;
    }

    nav {
      background: #222;
      padding: 15px;
      text-align: center;
    }

    nav a {
      color: white;
      margin: 0 20px;
      text-decoration: none;
      font-size: 18px;
    }

    nav a:hover {
      color: #00bcd4;
    }

    section {
      padding: 40px 20px;
    }

    #home {
      background: #007bff;
      color: white;
      text-align: center;
      padding: 80px 20px;
    }

    .container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background: white;
      padding: 15px;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      text-align: center;
    }

    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
    }

    .price {
      color: green;
      font-size: 18px;
      margin: 10px 0;
    }

    button {
      background: #007bff;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
    }

    button:hover {
      background: #0056b3;
    }

    .cart {
      background: white;
      padding: 20px;
      border-radius: 10px;
      margin-top: 20px;
    }

    input, textarea {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
    }

    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 15px;
    }
  </style>
</head>

<body>

<nav>
  <a href="#home">Home</a>
  <a href="#products">Products</a>
  <a href="#contact">Contact Us</a>
</nav>

<section id="home">
  <h1>Welcome to My Store 🛒</h1>
  <p>Best products at affordable prices!</p>
</section>

<section id="products">
  <h2>Our Products</h2>
  <div class="container">
    <div class="card">
      <img src="https://picsum.photos/300/200?1">
      <h3>Product 1</h3>
      <p class="price">₹500</p>
      <button onclick="addToCart('Product 1', 500)">Add to Cart</button>
    </div>

    <div class="card">
      <img src="https://picsum.photos/300/200?2">
      <h3>Product 2</h3>
      <p class="price">₹800</p>
      <button onclick="addToCart('Product 2', 800)">Add to Cart</button>
    </div>

    <div class="card">
      <img src="https://picsum.photos/300/200?3">
      <h3>Product 3</h3>
      <p class="price">₹1200</p>
      <button onclick="addToCart('Product 3', 1200)">Add to Cart</button>
    </div>
  </div>

  <div class="cart">
    <h2>Cart</h2>
    <ul id="cartItems"></ul>
    <h3>Total: ₹<span id="total">0</span></h3>
  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <form onsubmit="submitForm(event)">
    <input type="text" placeholder="Your Name" required>
    <input type="email" placeholder="Your Email" required>
    <textarea placeholder="Your Message" rows="4" required></textarea>
    <button type="submit">Send Message</button>
  </form>
</section>

<footer>
  © 2026 My Store | All Rights Reserved
</footer>

<script>
  let total = 0;

  function addToCart(product, price) {
    const cartItems = document.getElementById("cartItems");
    const li = document.createElement("li");
    li.textContent = product + " - ₹" + price;
    cartItems.appendChild(li);

    total += price;
    document.getElementById("total").textContent = total;
  }

  function submitForm(event) {
    event.preventDefault();
    alert("Message sent successfully!");
  }
</script>

</body>
</html>
```

## OUTPUT
<img width="1890" height="895" alt="Screenshot 2026-02-23 160506" src="https://github.com/user-attachments/assets/22f92852-799d-4583-b743-e2b16a59a2c1" />

<img width="1905" height="887" alt="Screenshot 2026-02-23 160516" src="https://github.com/user-attachments/assets/75450a73-3116-45cf-8ca5-80f69a502638" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
