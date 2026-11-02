# Ex02 Commercial Website
## Date:11/2/26
## Name : MADHESH I
## Reg No: 212224220055

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
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SmartShop - Online Shopping Website</title>
    <!-- Linking external CSS file -->
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header class="header">
        <div class="container nav-container">
            <!-- Website Logo -->
            <a href="#home" class="logo">
                <span class="logo-icon">&#128722;</span>
                Smart<span class="logo-accent">Shop</span>
            </a>

            <!-- Navigation Menu -->
            <nav class="navbar">
                <ul class="nav-links">
                    <li><a href="#home" class="nav-link">Home</a></li>
                    <li><a href="#products" class="nav-link">Products</a></li>
                    <li><a href="#about" class="nav-link">About Us</a></li>
                    <li><a href="#contact" class="nav-link">Contact</a></li>
                    <li><a href="#account" class="nav-link nav-btn">My Account</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
       
        <section id="home" class="hero-section">
            <div class="container hero-container">
                <!-- Hero Text Column -->
                <div class="hero-content">
                    <span class="badge">Exclusive Deals 2026</span>
                    <h1 class="hero-title">Welcome to <span class="highlight-blue">Smart</span><span class="highlight-orange">Shop</span></h1>
                    <p class="hero-desc">Discover quality products at affordable prices. Shop the latest electronics, stylish fashion, and premium accessories all in one trusted destination.</p>
                    <div class="hero-actions">
                        <a href="#products" class="btn btn-primary">Shop Now &#8594;</a>
                        <a href="#about" class="btn btn-secondary">Learn More</a>
                    </div>
                </div>

                <!-- Hero Image Column -->
                <div class="hero-image-wrapper">
                    <img src="https://images.unsplash.com/photo-1483985988355-763728e1935b?auto=format&fit=crop&w=800&q=80" 
                         alt="Online Shopping Fashion and Deals Banner" 
                         class="hero-img">
                </div>
            </div>
        </section>

        <!-- Store Benefits / Features Strip (Flexbox) -->
        <section class="features-section">
            <div class="container features-container">
                <div class="feature-box">
                    <div class="feature-icon">&#128666;</div>
                    <div class="feature-text">
                        <h3>Free &amp; Fast Shipping</h3>
                        <p>Orders over $50 deliver free</p>
                    </div>
                </div>
                <div class="feature-box">
                    <div class="feature-icon">&#128274;</div>
                    <div class="feature-text">
                        <h3>Secure Payments</h3>
                        <p>100% encrypted &amp; safe checkout</p>
                    </div>
                </div>
                <div class="feature-box">
                    <div class="feature-icon">&#9851;</div>
                    <div class="feature-text">
                        <h3>30-Day Easy Return</h3>
                        <p>Hassle-free money-back policy</p>
                    </div>
                </div>
                <div class="feature-box">
                    <div class="feature-icon">&#128222;</div>
                    <div class="feature-text">
                        <h3>24/7 Support</h3>
                        <p>Dedicated customer helpline</p>
                    </div>
                </div>
            </div>
        </section>

    
        <section id="products" class="products-section">
            <div class="container">
                <div class="section-title-wrap">
                    <h2 class="section-title">Featured Products</h2>
                    <p class="section-subtitle">Handpicked selection of top-selling products at unbeatable discounts.</p>
                    <div class="title-underline"></div>
                </div>

                <!-- Product Cards Flex Container -->
                <div class="product-cards-container">
                    <!-- Product Card 1 -->
                    <div class="product-card">
                        <span class="product-badge sale-badge">Sale -25%</span>
                        <div class="product-img-box">
                            <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?auto=format&fit=crop&w=600&q=80" 
                                 alt="Wireless Noise-Canceling Headphones" 
                                 class="product-img">
                        </div>
                        <div class="product-details">
                            <span class="product-category">Electronics</span>
                            <h3 class="product-name">Wireless Headphones</h3>
                            <div class="product-rating">&#9733;&#9733;&#9733;&#9733;&#9733; <span>(4.8)</span></div>
                            <div class="price-box">
                                <span class="current-price">$59.99</span>
                                <span class="old-price">$79.99</span>
                            </div>
                            <a href="#contact" class="btn btn-buy">Buy Now</a>
                        </div>
                    </div>

                    <!-- Product Card 2 -->
                    <div class="product-card">
                        <span class="product-badge hot-badge">Popular</span>
                        <div class="product-img-box">
                            <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?auto=format&fit=crop&w=600&q=80" 
                                 alt="Smart Fitness Watch" 
                                 class="product-img">
                        </div>
                        <div class="product-details">
                            <span class="product-category">Wearables</span>
                            <h3 class="product-name">Smart Fitness Watch</h3>
                            <div class="product-rating">&#9733;&#9733;&#9733;&#9733;&#9734; <span>(4.5)</span></div>
                            <div class="price-box">
                                <span class="current-price">$79.99</span>
                                <span class="old-price">$119.99</span>
                            </div>
                            <a href="#contact" class="btn btn-buy">Buy Now</a>
                        </div>
                    </div>

                    <!-- Product Card 3 -->
                    <div class="product-card">
                        <span class="product-badge sale-badge">Best Seller</span>
                        <div class="product-img-box">
                            <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?auto=format&fit=crop&w=600&q=80" 
                                 alt="Pro Sport Running Sneakers" 
                                 class="product-img">
                        </div>
                        <div class="product-details">
                            <span class="product-category">Footwear</span>
                            <h3 class="product-name">Pro Sport Sneakers</h3>
                            <div class="product-rating">&#9733;&#9733;&#9733;&#9733;&#9733; <span>(4.9)</span></div>
                            <div class="price-box">
                                <span class="current-price">$49.99</span>
                                <span class="old-price">$69.99</span>
                            </div>
                            <a href="#contact" class="btn btn-buy">Buy Now</a>
                        </div>
                    </div>

                    <!-- Product Card 4 -->
                    <div class="product-card">
                        <span class="product-badge hot-badge">Trending</span>
                        <div class="product-img-box">
                            <img src="https://images.unsplash.com/photo-1553062407-98eeb64c6a62?auto=format&fit=crop&w=600&q=80" 
                                 alt="Water-Resistant Travel Backpack" 
                                 class="product-img">
                        </div>
                        <div class="product-details">
                            <span class="product-category">Accessories</span>
                            <h3 class="product-name">Travel Backpack</h3>
                            <div class="product-rating">&#9733;&#9733;&#9733;&#9733;&#9734; <span>(4.6)</span></div>
                            <div class="price-box">
                                <span class="current-price">$39.99</span>
                                <span class="old-price">$55.00</span>
                            </div>
                            <a href="#contact" class="btn btn-buy">Buy Now</a>
                        </div>
                    </div>

                    <!-- Product Card 5 -->
                    <div class="product-card">
                        <div class="product-img-box">
                            <img src="https://images.unsplash.com/photo-1608156639585-b3a032ef9689?auto=format&fit=crop&w=600&q=80" 
                                 alt="Portable Bluetooth Speaker" 
                                 class="product-img">
                        </div>
                        <div class="product-details">
                            <span class="product-category">Audio</span>
                            <h3 class="product-name">Bluetooth Speaker</h3>
                            <div class="product-rating">&#9733;&#9733;&#9733;&#9733;&#9734; <span>(4.4)</span></div>
                            <div class="price-box">
                                <span class="current-price">$34.99</span>
                                <span class="old-price">$49.99</span>
                            </div>
                            <a href="#contact" class="btn btn-buy">Buy Now</a>
                        </div>
                    </div>

                    <!-- Product Card 6 -->
                    <div class="product-card">
                        <div class="product-img-box">
                            <img src="https://images.unsplash.com/photo-1572635196237-14b3f281503f?auto=format&fit=crop&w=600&q=80" 
                                 alt="Classic Polarized Sunglasses" 
                                 class="product-img">
                        </div>
                        <div class="product-details">
                            <span class="product-category">Fashion</span>
                            <h3 class="product-name">Classic Sunglasses</h3>
                            <div class="product-rating">&#9733;&#9733;&#9733;&#9733;&#9733; <span>(4.7)</span></div>
                            <div class="price-box">
                                <span class="current-price">$24.99</span>
                                <span class="old-price">$39.99</span>
                            </div>
                            <a href="#contact" class="btn btn-buy">Buy Now</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="about" class="about-section">
            <div class="container about-container">
                <!-- About Image Column -->
                <div class="about-image-wrapper">
                    <img src="https://images.unsplash.com/photo-1556742049-0a67c5574f73?auto=format&fit=crop&w=800&q=80" 
                         alt="About SmartShop Customer Service Team" 
                         class="about-img">
                </div>

                <!-- About Text Column -->
                <div class="about-content">
                    <span class="badge">Who We Are</span>
                    <h2 class="section-title">About SmartShop</h2>
                    <p class="about-text">
                        Founded with a simple mission in mind, <strong>SmartShop</strong> is dedicated to delivering superior products at prices everyone can afford. We believe that modern online shopping should be effortless, secure, and inspiring.
                    </p>
                    <p class="about-text">
                        From trending electronics and modern wardrobe staples to essential everyday lifestyle gear, we carefully curate each product from trusted manufacturers. Customer satisfaction is at the core of everything we build.
                    </p>

                    <!-- Highlights List (Flexbox) -->
                    <ul class="about-checklist">
                        <li><span class="check-icon">&#10004;</span> 100% Genuine and Certified Products</li>
                        <li><span class="check-icon">&#10004;</span> Transparent Pricing with Zero Hidden Costs</li>
                        <li><span class="check-icon">&#10004;</span> Dedicated 24/7 Human Support Team</li>
                        <li><span class="check-icon">&#10004;</span> Verified Customer Reviews and Secure Checkout</li>
                    </ul>

                    <a href="#products" class="btn btn-primary">Explore Products</a>
                </div>
            </div>
        </section>

        <section id="account" class="account-section">
            <div class="container">
                <div class="section-title-wrap">
                    <h2 class="section-title">My Account</h2>
                    <p class="section-subtitle">Sign in to track orders or register a new account to unlock member discounts.</p>
                    <div class="title-underline"></div>
                </div>

                <!-- Account Flex Container: Login & Register Cards Side-by-Side -->
                <div class="account-container">
                    <!-- Login Box -->
                    <div class="account-card">
                        <div class="card-header">
                            <span class="form-icon">&#128272;</span>
                            <h3>Login to Account</h3>
                            <p>Welcome back! Please enter your details.</p>
                        </div>
                        <form action="#" method="post" class="account-form">
                            <div class="form-group">
                                <label for="login-username">Username or Email</label>
                                <input type="text" id="login-username" name="login_username" placeholder="e.g. john@example.com" required>
                            </div>
                            <div class="form-group">
                                <label for="login-password">Password</label>
                                <input type="password" id="login-password" name="login_password" placeholder="Enter your password" required>
                            </div>
                            <div class="form-options">
                                <label class="checkbox-label">
                                    <input type="checkbox" name="remember"> Remember me
                                </label>
                                <a href="#account" class="forgot-link">Forgot password?</a>
                            </div>
                            <button type="submit" class="btn btn-primary btn-block">Login</button>
                        </form>
                    </div>

                    <!-- Register Box -->
                    <div class="account-card">
                        <div class="card-header">
                            <span class="form-icon">&#128100;</span>
                            <h3>Create New Account</h3>
                            <p>New to SmartShop? Create an account in seconds.</p>
                        </div>
                        <form action="#" method="post" class="account-form">
                            <div class="form-group">
                                <label for="reg-username">Username</label>
                                <input type="text" id="reg-username" name="reg_username" placeholder="Choose a username" required>
                            </div>
                            <div class="form-group">
                                <label for="reg-email">Email Address</label>
                                <input type="email" id="reg-email" name="reg_email" placeholder="yourname@example.com" required>
                            </div>
                            <div class="form-group">
                                <label for="reg-password">Password</label>
                                <input type="password" id="reg-password" name="reg_password" placeholder="Create a strong password" required>
                            </div>
                            <div class="form-options">
                                <label class="checkbox-label">
                                    <input type="checkbox" name="terms" required> I agree to the <a href="#">Terms &amp; Conditions</a>
                                </label>
                            </div>
                            <button type="submit" class="btn btn-secondary btn-block">Register</button>
                        </form>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact" class="contact-section">
            <div class="container">
                <div class="section-title-wrap">
                    <h2 class="section-title">Contact Us</h2>
                    <p class="section-subtitle">Have questions about an order or need help? Reach out to us anytime.</p>
                    <div class="title-underline"></div>
                </div>

                <!-- Contact Flex Container -->
                <div class="contact-container">
                    <!-- Contact Details Info Card -->
                    <div class="contact-info-card">
                        <h3>Get In Touch</h3>
                        <p class="info-intro">Our support team is always ready to assist you. Fill out the contact form or reach us directly.</p>

                        <div class="contact-item">
                            <div class="contact-item-icon">&#128231;</div>
                            <div class="contact-item-details">
                                <strong>Email Address:</strong>
                                <span>support@smartshop.com</span>
                            </div>
                        </div>

                        <div class="contact-item">
                            <div class="contact-item-icon">&#128222;</div>
                            <div class="contact-item-details">
                                <strong>Phone Number:</strong>
                                <span>+1 (800) 123-4567</span>
                            </div>
                        </div>

                        <div class="contact-item">
                            <div class="contact-item-icon">&#128205;</div>
                            <div class="contact-item-details">
                                <strong>Store Address:</strong>
                                <span>123 Commerce Boulevard, Suite 400, New York, NY 10001, USA</span>
                            </div>
                        </div>

                        <div class="contact-item">
                            <div class="contact-item-icon">&#9200;</div>
                            <div class="contact-item-details">
                                <strong>Operating Hours:</strong>
                                <span>Monday - Saturday: 9:00 AM - 8:00 PM</span>
                            </div>
                        </div>
                    </div>

                    <!-- Contact Form Card -->
                    <div class="contact-form-card">
                        <h3>Send a Message</h3>
                        <form action="#" method="post" class="contact-form">
                            <div class="form-group">
                                <label for="contact-name">Your Full Name</label>
                                <input type="text" id="contact-name" name="name" placeholder="John Doe" required>
                            </div>
                            <div class="form-group">
                                <label for="contact-email">Your Email Address</label>
                                <input type="email" id="contact-email" name="email" placeholder="john@example.com" required>
                            </div>
                            <div class="form-group">
                                <label for="contact-subject">Subject</label>
                                <input type="text" id="contact-subject" name="subject" placeholder="Question about an item / order" required>
                            </div>
                            <div class="form-group">
                                <label for="contact-message">Your Message</label>
                                <textarea id="contact-message" name="message" rows="5" placeholder="Write your inquiry or feedback here..." required></textarea>
                            </div>
                            <button type="submit" class="btn btn-primary btn-block">Submit Message &#10148;</button>
                        </form>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <footer class="footer">
        <div class="container footer-container">
            <!-- Footer Col 1: Brand -->
            <div class="footer-col brand-col">
                <a href="#home" class="logo footer-logo">
                    <span class="logo-icon">&#128722;</span>
                    Smart<span class="logo-accent">Shop</span>
                </a>
                <p class="footer-desc">
                    SmartShop is your premier online shopping destination. Delivering quality electronics, modern apparel, and accessories with trust and convenience.
                </p>
            </div>

            <!-- Footer Col 2: Navigation Links -->
            <div class="footer-col">
                <h4 class="footer-heading">Quick Links</h4>
                <ul class="footer-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#products">Products</a></li>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <li><a href="#account">My Account</a></li>
                </ul>
            </div>

            <!-- Footer Col 3: Customer Care -->
            <div class="footer-col">
                <h4 class="footer-heading">Customer Care</h4>
                <ul class="footer-links">
                    <li><a href="#about">Shipping Policy</a></li>
                    <li><a href="#about">Return &amp; Refund</a></li>
                    <li><a href="#about">Privacy Policy</a></li>
                    <li><a href="#contact">Help &amp; FAQs</a></li>
                    <li><a href="#account">Order Tracking</a></li>
                </ul>
            </div>

            <!-- Footer Col 4: Social Media Links -->
            <div class="footer-col">
                <h4 class="footer-heading">Follow Us</h4>
                <p class="social-text">Stay connected with our latest updates, offers and product launches:</p>
                <div class="social-links-box">
                    <a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="social-link instagram">
                        <span class="social-icon">&#128247;</span> Instagram
                    </a>
                    <a href="https://www.facebook.com" target="_blank" rel="noopener noreferrer" class="social-link facebook">
                        <span class="social-icon">&#128101;</span> Facebook
                    </a>
                    <a href="https://www.youtube.com" target="_blank" rel="noopener noreferrer" class="social-link youtube">
                        <span class="social-icon">&#9658;</span> YouTube
                    </a>
                </div>
            </div>
        </div>

        <!-- Copyright Bar -->
        <div class="footer-bottom">
            <div class="container footer-bottom-container">
                <p>&copy; 2026 SmartShop. All Rights Reserved. Built with HTML5 &amp; CSS3 Flexbox.</p>
            </div>
        </div>
    </footer>

</body>
</html>

```
style.css
```

:root {
    /* Primary & Secondary Color Palette */
    --color-primary: #1e3a8a;          /* Deep Navy Blue */
    --color-primary-light: #2563eb;    /* Bright Royal Blue */
    --color-primary-hover: #1d4ed8;    /* Darker Blue for button hover */
    --color-accent: #f97316;           /* Energetic Orange */
    --color-accent-hover: #ea580c;     /* Darker Orange for hover */

    /* Neutral Background & Surface Colors */
    --color-bg-white: #ffffff;         /* Pure White */
    --color-bg-light: #f8fafc;         /* Very Light Slate (section alternate) */
    --color-bg-card: #ffffff;          /* Card Background */
    --color-border: #e2e8f0;           /* Soft Border */
    --color-border-focus: #3b82f6;     /* Border glow on focus */

    /* Typography Colors */
    --color-text-dark: #0f172a;        /* Deep Slate / Charcoal */
    --color-text-body: #334155;        /* Neutral Slate for paragraphs */
    --color-text-muted: #64748b;       /* Muted Grey for captions/subtitles */
    --color-text-white: #ffffff;

    /* Typography & Spacing */
    --font-main: 'Segoe UI', system-ui, -apple-system, BlinkMacSystemFont, 'Roboto', 'Oxygen', 'Ubuntu', sans-serif;
    --radius-sm: 6px;
    --radius-md: 10px;
    --radius-lg: 16px;
    --radius-round: 50px;

    /* Shadows & Transitions */
    --shadow-sm: 0 2px 4px rgba(0, 0, 0, 0.05);
    --shadow-md: 0 4px 12px rgba(15, 23, 42, 0.08);
    --shadow-lg: 0 12px 28px rgba(15, 23, 42, 0.12);
    --transition-fast: all 0.25s ease-in-out;
}

/* Universal Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Smooth Scrolling for Section Links */
html {
    scroll-behavior: smooth;
}

body {
    font-family: var(--font-main);
    background-color: var(--color-bg-white);
    color: var(--color-text-body);
    line-height: 1.6;
    font-size: 16px;
    overflow-x: hidden;
}

/* Standard Content Container (Used everywhere for consistent width) */
.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 15px;
}

/* Images Default Behavior */
img {
    max-width: 100%;
    height: auto;
    display: block;
}

/* Links Reset */
a {
    text-decoration: none;
    color: inherit;
    transition: var(--transition-fast);
}

ul {
    list-style: none;
}

/* Headings Base Style */
h1, h2, h3, h4 {
    color: var(--color-text-dark);
    font-weight: 700;
    line-height: 1.25;
}

/* Section Header Titles */
.section-title-wrap {
    text-align: center;
    margin-bottom: 45px;
}

.section-title {
    font-size: 2.2rem;
    color: var(--color-primary);
    margin-bottom: 8px;
}

.section-subtitle {
    color: var(--color-text-muted);
    font-size: 1.05rem;
    max-width: 600px;
    margin: 0 auto;
}

.title-underline {
    width: 60px;
    height: 4px;
    background-color: var(--color-accent);
    margin: 12px auto 0;
    border-radius: var(--radius-round);
}

/* Reusable Badges */
.badge {
    display: inline-block;
    padding: 6px 14px;
    font-size: 0.82rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    background-color: rgba(37, 99, 235, 0.1);
    color: var(--color-primary-light);
    border-radius: var(--radius-round);
    margin-bottom: 12px;
}

/* Color Accent Text Spans */
.highlight-blue {
    color: var(--color-primary);
}

.highlight-orange {
    color: var(--color-accent);
}

.btn {
    display: inline-block;
    padding: 12px 26px;
    font-size: 0.98rem;
    font-weight: 600;
    border-radius: var(--radius-round);
    border: 2px solid transparent;
    cursor: pointer;
    text-align: center;
    transition: var(--transition-fast);
}

.btn-primary {
    background-color: var(--color-accent);
    color: var(--color-text-white);
    box-shadow: 0 4px 12px rgba(249, 115, 22, 0.3);
}

.btn-primary:hover {
    background-color: var(--color-accent-hover);
    transform: translateY(-2px);
    box-shadow: 0 6px 16px rgba(249, 115, 22, 0.4);
}

.btn-secondary {
    background-color: transparent;
    color: var(--color-primary);
    border-color: var(--color-primary);
}

.btn-secondary:hover {
    background-color: var(--color-primary);
    color: var(--color-text-white);
    transform: translateY(-2px);
    box-shadow: 0 6px 16px rgba(30, 58, 138, 0.25);
}

.btn-buy {
    background-color: var(--color-primary);
    color: var(--color-text-white);
    padding: 10px 20px;
    font-size: 0.9rem;
    border-radius: var(--radius-sm);
    width: 100%;
}

.btn-buy:hover {
    background-color: var(--color-accent);
    transform: translateY(-2px);
}

.btn-block {
    width: 100%;
    margin-top: 10px;
}


.header {
    background-color: var(--color-bg-white);
    box-shadow: var(--shadow-sm);
    position: sticky;
    top: 0;
    z-index: 1000;
    border-bottom: 1px solid var(--color-border);
}

/* CSS FLEXBOX: Distribute logo on left and navbar links on right */
.nav-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 16px;
    padding-bottom: 16px;
}

/* Logo Styling */
.logo {
    font-size: 1.6rem;
    font-weight: 800;
    color: var(--color-primary);
    display: flex;
    align-items: center;
    gap: 8px;
    letter-spacing: -0.5px;
}

.logo-icon {
    font-size: 1.6rem;
    color: var(--color-accent);
}

.logo-accent {
    color: var(--color-accent);
}

/* CSS FLEXBOX: Align navigation menu horizontally */
.nav-links {
    display: flex;
    align-items: center;
    gap: 24px;
}

.nav-link {
    font-size: 0.98rem;
    font-weight: 600;
    color: var(--color-text-dark);
    padding: 8px 12px;
    border-radius: var(--radius-sm);
    position: relative;
}

/* Navigation Hover Effect with Accent Indicator */
.nav-link:hover {
    color: var(--color-accent);
}

.nav-link::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    width: 0;
    height: 2px;
    background-color: var(--color-accent);
    transition: var(--transition-fast);
    transform: translateX(-50%);
}

.nav-link:hover::after {
    width: 80%;
}

/* Special button style for "My Account" link in nav */
.nav-btn {
    background-color: var(--color-primary);
    color: var(--color-text-white) !important;
    padding: 8px 18px;
    border-radius: var(--radius-round);
}

.nav-btn::after {
    display: none;
}

.nav-btn:hover {
    background-color: var(--color-accent);
    color: var(--color-text-white);
    transform: translateY(-2px);
    box-shadow: 0 4px 10px rgba(249, 115, 22, 0.3);
}


.hero-section {
    padding: 60px 0 70px;
    background: linear-gradient(135deg, #f8fafc 0%, #eff6ff 100%);
    border-bottom: 1px solid var(--color-border);
}

/* CSS FLEXBOX: Two column layout with text and banner image */
.hero-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
}

.hero-content {
    flex: 1;
}

.hero-title {
    font-size: 3rem;
    margin-bottom: 18px;
    line-height: 1.15;
}

.hero-desc {
    font-size: 1.15rem;
    color: var(--color-text-body);
    margin-bottom: 28px;
    max-width: 520px;
}

/* CSS FLEXBOX: Horizontal alignment for Call-To-Action buttons */
.hero-actions {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
}

.hero-image-wrapper {
    flex: 1;
    display: flex;
    justify-content: center;
}

.hero-img {
    width: 100%;
    max-width: 520px;
    height: 380px;
    object-fit: cover;
    border-radius: var(--radius-lg);
    box-shadow: var(--shadow-lg);
    border: 4px solid var(--color-bg-white);
    transition: transform 0.4s ease;
}

.hero-img:hover {
    transform: scale(1.02);
}


.features-section {
    padding: 30px 0;
    background-color: var(--color-bg-white);
    border-bottom: 1px solid var(--color-border);
}

/* CSS FLEXBOX: Distribute 4 feature cards evenly */
.features-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
}

.feature-box {
    display: flex;
    align-items: center;
    gap: 14px;
    flex: 1 1 220px;
    padding: 12px;
}

.feature-icon {
    font-size: 2rem;
    color: var(--color-primary-light);
    background-color: #eff6ff;
    width: 54px;
    height: 54px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
}

.feature-text h3 {
    font-size: 1rem;
    margin-bottom: 2px;
}

.feature-text p {
    font-size: 0.85rem;
    color: var(--color-text-muted);
}


.products-section {
    padding: 80px 0;
    background-color: var(--color-bg-white);
}

/* CSS FLEXBOX: Multi-row wrap alignment for product catalog */
.product-cards-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
}

/* Individual Product Card */
.product-card {
    background-color: var(--color-bg-card);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-md);
    width: 270px;
    padding: 16px;
    position: relative;
    box-shadow: var(--shadow-sm);
    /* CSS FLEXBOX: Stacks product elements vertically with even spacing */
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    transition: transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s ease;
}

/* Product Card Hover Effect */
.product-card:hover {
    transform: translateY(-8px);
    box-shadow: var(--shadow-lg);
    border-color: #cbd5e1;
}

/* Promotional Badges */
.product-badge {
    position: absolute;
    top: 12px;
    left: 12px;
    font-size: 0.75rem;
    font-weight: 700;
    padding: 4px 10px;
    border-radius: var(--radius-round);
    z-index: 2;
    text-transform: uppercase;
}

.sale-badge {
    background-color: var(--color-accent);
    color: var(--color-text-white);
}

.hot-badge {
    background-color: var(--color-primary-light);
    color: var(--color-text-white);
}

/* Product Image Box */
.product-img-box {
    width: 100%;
    height: 200px;
    border-radius: var(--radius-sm);
    overflow: hidden;
    margin-bottom: 14px;
    background-color: #f1f5f9;
}

.product-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.4s ease;
}

.product-card:hover .product-img {
    transform: scale(1.06);
}

/* Product Information */
.product-details {
    display: flex;
    flex-direction: column;
    gap: 6px;
}

.product-category {
    font-size: 0.78rem;
    color: var(--color-text-muted);
    text-transform: uppercase;
    font-weight: 600;
    letter-spacing: 0.5px;
}

.product-name {
    font-size: 1.1rem;
    color: var(--color-text-dark);
}

.product-rating {
    color: #eab308; /* Star Gold */
    font-size: 0.9rem;
}

.product-rating span {
    color: var(--color-text-muted);
    font-size: 0.8rem;
    margin-left: 4px;
}

/* CSS FLEXBOX: Align current price and crossed-out old price */
.price-box {
    display: flex;
    align-items: baseline;
    gap: 8px;
    margin: 8px 0 12px;
}

.current-price {
    font-size: 1.3rem;
    font-weight: 700;
    color: var(--color-accent);
}

.old-price {
    font-size: 0.9rem;
    color: var(--color-text-muted);
    text-decoration: line-through;
}


.about-section {
    padding: 80px 0;
    background-color: var(--color-bg-light);
    border-top: 1px solid var(--color-border);
    border-bottom: 1px solid var(--color-border);
}

/* CSS FLEXBOX: Side-by-side image and story column */
.about-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 50px;
}

.about-image-wrapper {
    flex: 1;
}

.about-img {
    width: 100%;
    max-width: 520px;
    height: 400px;
    object-fit: cover;
    border-radius: var(--radius-
}

.about-content {
    flex: 1;
}
lg);
    box-shadow: var(--shadow-md);
    border: 4px solid var(--color-bg-white);
.about-content .section-title {
    text-align: left;
    margin-bottom: 16px;
}

```
## OUTPUT
![alt text](<assests/Screenshot (530).png>)
![alt text](<assests/Screenshot (531).png>)
![alt text](<assests/Screenshot (532).png>)
![alt text](<assests/Screenshot (533).png>)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.