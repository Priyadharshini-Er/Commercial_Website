# Ex02 Commercial Website
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

## HTML
```
<!DOCTYPE html>
<html>
<head>
    <title>Login - GlowCare</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
<header>
    <h1>GlowCare</h1>
    <nav>
        <a href="login.html">Login</a>
        <a href="index.html">Home</a>
        <a href="shop.html">Shop</a>
        <a href="about.html">About Us</a>
        <a href="contact.html">Contact</a>
    </nav>
</header>

<div class="container">
   <section id="login">
    <h2>Login</h2>
    <form class="login-form">
        <label for="email">Email:</label>
        <input type="email" id="email" name="email">

        <label for="password">Password:</label>
        <input type="password" id="password" name="password">

        <button type="submit">Login</button>
    </form>
</section>
</div>


  <div class="container">
        <h2>Welcome to GlowCare</h2>
        <p class="center-text">Your one-stop shop for natural, skin-friendly products.</p>
        <img src="image2.jpeg" alt="Skincare Banner" style="width:100%">
    </div>

    <div class="products-container">
    <div class="product">
        <img src="img.jpeg" alt="Vitamin C Serum">
        <p>Vitamin-C brightning serum - $40</p>
    </div>
    <div class="product">
        <img src="img2.jpeg" alt="Sunscreen">
        <p>Aqualogica Glow + Dewy Sunscreen - $50</p>
    </div>
    <div class="product">
        <img src="facewash.jpeg" alt="Facewash">
        <p>Cetaphil Oily Skin Cleanser - $17</p>
    </div>
    <div class="product">
        <img src="moist.jpeg" alt="Moisturizer">
        <p>2% Niacinamide & Rice Water Brightening Gel Moisturizer - $24</p>
    </div>
    <div class="product">
        <img src="Lotion.jpeg" alt="Body Lotion">
        <p>Vanilla Caramello Body Lotion by Plum BodyLovin' - $20</p>
    </div>
    <div class="product">
        <img src="eyeserum.jpeg" alt="Eye Serum">
        <p>Hydra Eye Serum Patch with Coffee - $15</p>
    </div>
</div>

<div class="container">
    <h2>About GlowCare</h2>
    <img src="abtus.jpeg" alt="GlowCare Logo" style="width: 100%">
    <p>GlowCare is dedicated to creating natural skincare products that nourish your skin. We believe in purity, transparency, and eco-friendly practices.</p>

    <p>Our products are made with the finest ingredients, carefully selected to provide the best results</p>

    <p>GlowCare is an Indian self-care brand that’s all about offering clean, cruelty-free products. We’re here to make your skincare routine go from “meh” to wow, delivering radiant results that speak for themselves.</p>

    <P><b>Our vision is simple yet bold:</b> To make luxury skincare accessible to everyone. We create products that work wonders for your skin & are also gentle (even for the planet). It's all about offering affordable luxury without compromise because you deserve to glow every day</p>
</div>

<div class="container">
    <section id="contact">
    <h2>Contact Us</h2>
    <form class="contact-form">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name">

        <label for="email">Email:</label>
        <input type="email" id="email" name="email">

        <label for="message">Message:</label>
        <textarea id="message" name="message" rows="4"></textarea>

        <button type="submit">Send</button>
    </form>
    <p> For booking details please contact us through what's app</p>
    <p><b>what's app number : 98524 14675</b></p>
</section>
</div>

<footer>
    &copy; 2025 GlowCare. All rights reserved.
</footer>
</body>
</html>
```

## CSS

```
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background-color: #fff9f8;
    color: #333;
}

h2{
    text-align: center;
}


p {
    text-align: center;
}


header {
    background-color: #f7d1c8;
    padding: 15px 0;
    text-align: center;
}

nav a {
    text-decoration: none;
    color: #333;
    margin: 0 15px;
    font-weight: bold;
}

nav a:hover {
    color: #d17c6c;
}

.products-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr); 
    gap: 20px;
    justify-items: center; 
}

.product {
    text-align: center; 
}
.product img {
    max-width: 120px; 
}

#contact {
    text-align: center; 
    padding: 40px 20px;
}

.contact-form {
    display: flex;
    flex-direction: column;
    align-items: center;   
    justify-content: center;
    max-width: 400px;      
    margin: 0 auto;        
}

.contact-form label {
    align-self: flex-start;
    margin: 5px 0 3px;
}

.contact-form input,
.contact-form textarea {
    width: 100%;
    padding: 8px;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.contact-form button {
    padding: 10px 20px;
    border: none;
    background-color: #333;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

.contact-form button:hover {
    background-color: #555;
}

/* Login Section */
#login {
    text-align: center;  /* centers the heading */
    padding: 40px 20px;
}

.login-form {
    display: flex;
    flex-direction: column;
    align-items: center;   /* centers form horizontally */
    justify-content: center;
    max-width: 350px;      /* limit width */
    margin: 0 auto;        /* centers inside page */
    background: #fff;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}

.login-form label {
    align-self: flex-start;
    margin: 5px 0 3px;
}

.login-form input {
    width: 100%;
    padding: 8px;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.login-form button {
    padding: 10px 20px;
    border: none;
    background-color: #333;
    color: white;
    border-radius: 5px;
    cursor: pointer;
}

.login-form button:hover {
    background-color: #555;
}

footer {
    text-align: center;
    background: #f7d1c8;
    padding: 10px;
    margin-top: 20px;
}
```

## OUTPUT

<img width="1365" height="564" alt="image" src="https://github.com/user-attachments/assets/f5d02754-3ac8-4c44-bf31-d67bbaffcf5d" />

<img width="1365" height="662" alt="image" src="https://github.com/user-attachments/assets/71912d26-536e-4f2a-a7f1-08de98a48eac" />

<img width="1365" height="610" alt="image" src="https://github.com/user-attachments/assets/2ea2e244-c2ac-44a5-b05e-e6e645819b58" />

<img width="1365" height="679" alt="image" src="https://github.com/user-attachments/assets/e890cf08-3986-4968-b6c4-b55556dba855" />

<img width="1363" height="480" alt="image" src="https://github.com/user-attachments/assets/0bd3484c-56f2-4f54-9a1b-77a5bac63822" />

<img width="1364" height="663" alt="image" src="https://github.com/user-attachments/assets/d9c03e44-9eec-4fcd-b2d6-b8cff939eb22" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
