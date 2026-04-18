# Emperor-meme.github.io
/* Ensure the modal covers everything */
#auth-modal {
    position: fixed;
    top: 0; left: 0; 
    width: 100%; height: 100%;
    background: #051937; /* Dark background */
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 9999;
}

.auth-box {
    background: #000a1f;
    padding: 30px;
    border-radius: 15px;
    border: 1px solid #00bcd4;
    text-align: center;
    width: 300px;
}

.auth-box input {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border-radius: 5px;
    border: 1px solid #333;
    background: #111;
    color: white;
    box-sizing: border-box; /* Ensures padding doesn't break layout */
}

.auth-btn {
    background: #00bcd4;
    color: #051937;
    padding: 10px;
    border: none;
    border-radius: 5px;
    font-weight: bold;
    cursor: pointer;
    width: 100%;
    margin-top: 10px;
}
/* style.css - Updated for Hosted Images */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #051937;
    /* Slanted light blue strokes background effect */
    background-image: 
        linear-gradient(135deg, rgba(168, 218, 220, 0.1) 25%, transparent 25%),
        linear-gradient(225deg, rgba(168, 218, 220, 0.1) 25%, transparent 25%),
        linear-gradient(135deg, transparent 75%, rgba(168, 218, 220, 0.1) 75%),
        linear-gradient(225deg, transparent 75%, rgba(168, 218, 220, 0.1) 75%);
    background-size: 80px 80px;
    color: #f0f0f0;
    line-height: 1.6;
    min-height: 100vh;
}

/* Header */
header {
    background: #000a1f;
    padding: 10px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0 2px 10px rgba(0,0,0,0.5);
    position: sticky;
    top: 0;
    z-index: 1000;
}

#logo-text {
    font-size: 1.5rem;
    font-weight: bold;
    color: #00bcd4;
    text-decoration: none;
}

nav a {
    color: #d8e6f3;
    margin: 0 15px;
    text-decoration: none;
    font-weight: 600;
}

nav a:hover {
    color: #00bcd4;
}

/* Universal Page Containers */
.container {
    max-width: 1100px;
    margin: 30px auto;
    padding: 20px;
}

h1, h2 {
    color: #e0f2fe;
    margin-bottom: 20px;
}

p {
    margin-bottom: 15px;
    color: #c0d1e3;
}

/* Image styling */
.img-fluid {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}

/* Updated Hero Section with Blurred Online Image */
.hero-section {
    position: relative;
    padding: 100px 40px;
    margin-bottom: 50px;
    border-radius: 12px;
    overflow: hidden;
    text-align: center;
}

/* The online image used as the hero background */
.hero-bg-image {
    position: absolute;
    top: 0; left: 0; width: 100%; height: 100%;
    background-size: cover;
    background-position: center;
    filter: blur(4px) brightness(0.4); /* Darkens and blurs background */
    z-index: 1;
}

.hero-text-overlay {
    position: relative;
    z-index: 2; /* Sits on top of the blurred image */
}

/* Second Happy People Section styling */
.people-section {
    display: flex;
    align-items: center;
    gap: 40px;
    background: rgba(0, 10, 31, 0.6);
    padding: 40px;
    border-radius: 12px;
    margin-bottom: 50px;
}

.people-text, .people-img { flex: 1; }

/* Cards */
.interactive-cards { display: flex; gap: 20px; margin-bottom: 50px; }
.card {
    flex: 1;
    background: rgba(255,255,255,0.05);
    padding: 25px;
    border-radius: 10px;
    border: 1px solid rgba(0, 188, 212, 0.2);
    transition: transform 0.3s;
}
.card:hover { transform: translateY(-5px); border-color: #00bcd4; }
.card h3 { color: #00bcd4; margin-bottom: 10px; }

/* Grid for other pages */
.info-grid { display: flex; flex-wrap: wrap; gap: 30px; margin-top: 30px; }
.info-item { flex: 1 1 300px; background: rgba(0, 10, 31, 0.6); padding: 20px; border-radius: 8px; }

/* Buttons & Links */
.btn {
    display: inline-block; background: #25d366; color: white;
    padding: 12px 24px; text-decoration: none; border-radius: 30px;
    font-weight: bold; font-size: 1.1rem; transition: transform 0.2s;
    box-shadow: 0 4px 10px rgba(0,0,0,0.2);
}
.btn:hover { transform: scale(1.05); background: #1eb956; }
.contact-link { color: #e0f2fe; text-decoration: none; font-weight: bold; }
.payment-details { background: rgba(0, 188, 212, 0.1); border-left: 5px solid #00bcd4; padding: 20px; border-radius: 5px; }




<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Emperors Lounge | Premium Laptops</title>
</head>
<body>
    <header>
    <a href="index.html" id="logo-text">E. LOUNGE</a>
    <nav>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
        <a href="services.html">Services</a>
        <a href="payment.html">Payment</a>
        <span id="display-email" style="color: #00bcd4; font-size: 0.8rem; margin-left: 10px;"></span>
        <button onclick="logoutUser()" style="background: transparent; border: 1px solid #ff4d4d; color: #ff4d4d; padding: 5px 10px; border-radius: 5px; cursor: pointer; margin-left: 10px;">Logout</button>
    </nav>
</header>
    <script>
    // 1. Check if user is logged in on page load
    window.onload = function() {
        if(localStorage.getItem('isLoggedIn') === 'true') {
            document.getElementById('auth-modal').style.display = 'none';
        }
    };

    function validateAccess() {
    const email = document.getElementById('email').value;
    const pass = document.getElementById('password').value;
    if (email.includes('@') && email.length > 5 && pass.length >= 6) {
        localStorage.setItem('isLoggedIn', 'true');
        localStorage.setItem('userEmail', email); // Save the email here
        document.getElementById('auth-modal').style.display = 'none';
        location.reload(); // Refresh to show the email immediately
    } else { alert("Please enter a valid email and a password of at least 6 characters."); }
}
</script>
<div id="auth-modal">
    <div class="auth-box">
        <h2 id="auth-title">Emperors Lounge</h2>
        <input type="text" id="email" placeholder="Email Address">
        <input type="password" id="password" placeholder="Password (min 6 chars)">
        
        <button class="auth-btn" onclick="validateAccess()">Sign In / Create Account</button>
        
        <p style="font-size: 0.8rem; margin-top: 10px; color: #888;">
            Access is restricted to authorized users.
        </p>
    </div>
</div>

    <div class="container">
        <section class="hero-section">
            <div class="hero-bg-image" style="background-image: url('https://images.unsplash.com/photo-1499951360447-b19be8fe80f5?q=80&w=1200');"></div>
            
            <div class="hero-text-overlay">
                <h1>Unlock the Power of Computing</h1>
                <p>Welcome to <strong>Emperors Lounge</strong>. Technology should empower you. Laptops are your gateway to creativity, business growth, research, and communication.</p>
                <p>We match you with the right processor, memory, and performance needed for your journey.</p>
                <a href="https://wa.me/2348136693871" class="btn">Chat on WhatsApp</a>
            </div>
        </section>

        <section class="interactive-cards">
            <div class="card">
                <h3>Processors (CPU)</h3>
                <p>The "brain" of your laptop. Faster processors like Intel Core i7 or Ryzen 7 can handle video editing and gaming effortlessly. We find the sweet spot for your workload.</p>
            </div>
            <div class="card">
                <h3>Memory (RAM)</h3>
                <p>The short-term memory that keeps your machine fast when many tabs are open. 8GB is standard, but we recommend 16GB for heavy multitasking.</p>
            </div>
            <div class="card">
                <h3>Storage (SSD)</h3>
                <p>Where your files live. We only stock laptops with Solid State Drives (SSDs). SSDs are much faster and more durable than old Hard Disk Drives (HDDs).</p>
            </div>
        </section>

        <section class="people-section">
            <div class="people-img">
                <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?q=80&w=800" alt="Happy clients with computers" class="img-fluid">
            </div>
            <div class="people-text">
                <h2>Our Client Commitment</h2>
                <p>Our goal is to see you smile. Whether you are a student preparing for JAMB (good luck with your physics preparation!) or a business professional, having reliable hardware shouldn't be stressful.</p>
                <p>We provide durable machines that guarantee reliability, speed, and great battery life, allowing you to focus on your success.</p>
                <p>Reach us anytime via Email: <a href="mailto:yungchidex333@gmail.com" class="contact-link">yungchidex333@gmail.com</a></p>
            </div>
        </section>

    </div>
<script>
    // Logic to check if user is logged in
    window.onload = function() { 
        if(localStorage.getItem('isLoggedIn') === 'true') { 
            document.getElementById('auth-modal').style.display = 'none';
            document.getElementById('display-email').innerText = localStorage.getItem('userEmail');
        } 
    };

    // Logic to sign in
    function validateAccess() {
        const email = document.getElementById('email').value;
        const pass = document.getElementById('password').value;
        if(email.includes('@') && email.length > 5 && pass.length >= 6) {
            localStorage.setItem('isLoggedIn', 'true');
            localStorage.setItem('userEmail', email);
            document.getElementById('auth-modal').style.display = 'none';
            location.reload();
        } else { 
            alert("Please enter a valid email and a password of at least 6 characters."); 
        }
    }

    // Logic to logout
    function logoutUser() {
        localStorage.removeItem('isLoggedIn');
        localStorage.removeItem('userEmail');
        location.reload();
    }
</script>
</body>
</html>






<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Secure Payment Details</title>
</head>
<body>
    <header>
        <a href="index.html" id="logo-text">
            E. LOUNGE
        </a>
        ...
        <nav>
            <a href="index.html">Home</a>
            <a href="about.html">About</a>
            <a href="services.html">Services</a>
            <a href="payment.html">Payment</a>
             <span id="display-email" style="color: #00bcd4; font-size: 0.8rem; margin-left: 10px;"></span>
             <button onclick="logoutUser()" style="background: transparent; border: 1px solid #ff4d4d; color: #ff4d4d; padding: 5px 10px; border-radius: 5px; cursor: pointer; margin-left: 10px;">Logout</button>
        </nav>
    </header>
     <script>
    // 1. Check if user is logged in on page load
    window.onload = function() {
        if(localStorage.getItem('isLoggedIn') === 'true') {
            document.getElementById('auth-modal').style.display = 'none';
        }
    };

    function validateAccess() {
    const email = document.getElementById('email').value;
    const pass = document.getElementById('password').value;
    if (email.includes('@') && email.length > 5 && pass.length >= 6) {
        localStorage.setItem('isLoggedIn', 'true');
        localStorage.setItem('userEmail', email); // Save the email here
        document.getElementById('auth-modal').style.display = 'none';
        location.reload(); // Refresh to show the email immediately
    } else { alert("Please enter a valid email and a password of at least 6 characters."); }
}
</script>
<div id="auth-modal">
    <div class="auth-box">
        <h2 id="auth-title">Emperors Lounge</h2>
        <input type="text" id="email" placeholder="Email Address">
        <input type="password" id="password" placeholder="Password (min 6 chars)">
        
        <button class="auth-btn" onclick="validateAccess()">Sign In / Create Account</button>
        
        <p style="font-size: 0.8rem; margin-top: 10px; color: #888;">
            Access is restricted to authorized users.
        </p>
    </div>
</div>

    <div class="container">
        <h1>Payment & Transfer Details</h1>
        <div class="info-grid">
            <div class="info-item">
                <h2>Secure Your Order</h2>
                <p>Thank you for choosing Emperors Lounge. We aim to keep your transaction seamless and secure.</p>
                <p>Please use the transfer details provided. Once your payment is completed, please take a screenshot or proof of payment and send it directly to our WhatsApp number so we can process your order immediately.</p>
            </div>
            
            <div class="info-item payment-details">
                <h2>Transfer Details</h2>
                <p><strong>Bank:</strong> OPay</p>
                <p><strong>Account Name:</strong> LIVINUS CHUKWU OGBU</p>
                <p><strong>Account Number:</strong> 8153317031</p>
            </div>
        </div>
         <center>
            <a href="https://wa.me/2348136693871" class="btn" style="background:#e0f2fe; color:#051937;">Confirm Payment on WhatsApp</a>
        </center>
    </div>
<script>
    // Logic to check if user is logged in
    window.onload = function() {
        if (localStorage.getItem('isLoggedIn') === 'true') {
            document.getElementById('auth-modal').style.display = 'none';
            document.getElementById('display-email').innerText = localStorage.getItem('userEmail');
        }
    };
    
    // Logic to sign in
    function validateAccess() {
        const email = document.getElementById('email').value;
        const pass = document.getElementById('password').value;
        if (email.includes('@') && email.length > 5 && pass.length >= 6) {
            localStorage.setItem('isLoggedIn', 'true');
            localStorage.setItem('userEmail', email);
            document.getElementById('auth-modal').style.display = 'none';
            location.reload();
        } else {
            alert("Please enter a valid email and a password of at least 6 characters.");
        }
    }
    
    // Logic to logout
    function logoutUser() {
        localStorage.removeItem('isLoggedIn');
        localStorage.removeItem('userEmail');
        location.reload();
    }
</script>
</body>
</html>







<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Our Services</title>
</head>
<body>
   <header>
    <a href="index.html" id="logo-text">E. LOUNGE</a>
    <nav>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
        <a href="services.html">Services</a>
        <a href="payment.html">Payment</a>
        <span id="display-email" style="color: #00bcd4; font-size: 0.8rem; margin-left: 10px;"></span>
        <button onclick="logoutUser()" style="background: transparent; border: 1px solid #ff4d4d; color: #ff4d4d; padding: 5px 10px; border-radius: 5px; cursor: pointer; margin-left: 10px;">Logout</button>
    </nav>
</header>
    <script>
    // 1. Check if user is logged in on page load
    window.onload = function() {
        if(localStorage.getItem('isLoggedIn') === 'true') {
            document.getElementById('auth-modal').style.display = 'none';
        }
    };

    function validateAccess() {
    const email = document.getElementById('email').value;
    const pass = document.getElementById('password').value;
    if (email.includes('@') && email.length > 5 && pass.length >= 6) {
        localStorage.setItem('isLoggedIn', 'true');
        localStorage.setItem('userEmail', email); // Save the email here
        document.getElementById('auth-modal').style.display = 'none';
        location.reload(); // Refresh to show the email immediately
    } else { alert("Please enter a valid email and a password of at least 6 characters."); }
}
</script>
<div id="auth-modal">
    <div class="auth-box">
        <h2 id="auth-title">Emperors Lounge</h2>
        <input type="text" id="email" placeholder="Email Address">
        <input type="password" id="password" placeholder="Password (min 6 chars)">
        
        <button class="auth-btn" onclick="validateAccess()">Sign In / Create Account</button>
        
        <p style="font-size: 0.8rem; margin-top: 10px; color: #888;">
            Access is restricted to authorized users.
        </p>
    </div>
</div>

    <div class="container">
        <h1>Laptop Sales & Services</h1>
        <div class="interactive-cards">
            <div class="card">
                <h3>Hardware Sales</h3>
                <p>Direct sales of high-performance laptops. We feature top brands including Dell, HP, Lenovo, and Apple, covering all specifications from basic study machines to powerful workstations.</p>
            </div>
            <div class="card">
                <h3>Tech Consultation</h3>
                <p>Need advice on upgrading? Unsure if you need an SSD upgrade or more RAM? We offer professional consulting to enhance your existing equipment or find the perfect replacement.</p>
            </div>
            <div class="card">
                <h3>Refurbished Excellence</h3>
                <p>Get premium performance at a lower cost. Our certified refurbished laptops are rigorously tested to ensure functionality, giving you 'like-new' reliability on a budget.</p>
            </div>
        </div>
        <center>
            <a href="https://wa.me/2348136693871" class="btn">Message Us for Availability</a>
        </center>
    </div>
    <script>
    // Logic to check if user is logged in
    window.onload = function() {
        if (localStorage.getItem('isLoggedIn') === 'true') {
            document.getElementById('auth-modal').style.display = 'none';
            document.getElementById('display-email').innerText = localStorage.getItem('userEmail');
        }
    };
    
    // Logic to sign in
    function validateAccess() {
        const email = document.getElementById('email').value;
        const pass = document.getElementById('password').value;
        if (email.includes('@') && email.length > 5 && pass.length >= 6) {
            localStorage.setItem('isLoggedIn', 'true');
            localStorage.setItem('userEmail', email);
            document.getElementById('auth-modal').style.display = 'none';
            location.reload();
        } else {
            alert("Please enter a valid email and a password of at least 6 characters.");
        }
    }
    
    // Logic to logout
    function logoutUser() {
        localStorage.removeItem('isLoggedIn');
        localStorage.removeItem('userEmail');
        location.reload();
    }
</script>
</body>
</html>






<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>About Emperors Lounge</title>
</head>
<body>
<header>
    <a href="index.html" id="logo-text">E. LOUNGE</a>
    <nav>
        <a href="index.html">Home</a>
        <a href="about.html">About</a>
        <a href="services.html">Services</a>
        <a href="payment.html">Payment</a>
        <span id="display-email" style="color: #00bcd4; font-size: 0.8rem; margin-left: 10px;"></span>
        <button onclick="logoutUser()" style="background: transparent; border: 1px solid #ff4d4d; color: #ff4d4d; padding: 5px 10px; border-radius: 5px; cursor: pointer; margin-left: 10px;">Logout</button>
    </nav>
</header>
    <script>
    // 1. Check if user is logged in on page load
    window.onload = function() {
        if(localStorage.getItem('isLoggedIn') === 'true') {
            document.getElementById('auth-modal').style.display = 'none';
        }
    };

    function validateAccess() {
    const email = document.getElementById('email').value;
    const pass = document.getElementById('password').value;
    if (email.includes('@') && email.length > 5 && pass.length >= 6) {
        localStorage.setItem('isLoggedIn', 'true');
        localStorage.setItem('userEmail', email); // Save the email here
        document.getElementById('auth-modal').style.display = 'none';
        location.reload(); // Refresh to show the email immediately
    } else { alert("Please enter a valid email and a password of at least 6 characters."); }
}
</script>
<div id="auth-modal">
    <div class="auth-box">
        <h2 id="auth-title">Emperors Lounge</h2>
        <input type="text" id="email" placeholder="Email Address">
        <input type="password" id="password" placeholder="Password (min 6 chars)">
        
        <button class="auth-btn" onclick="validateAccess()">Sign In / Create Account</button>
        
        <p style="font-size: 0.8rem; margin-top: 10px; color: #888;">
            Access is restricted to authorized users.
        </p>
    </div>
</div>

    <div class="container">
        <h1>About Emperors Lounge</h1>
        <div class="info-grid">
            <div class="info-item">
                <h2>Our Philosophy</h2>
                <p>Founded on principles of integrity and excellence, Emperors Lounge exists to bridge the gap between quality technology and everyday people.</p>
                <p>We understand that purchasing a laptop is a significant investment. Our philosophy is rooted in ensuring that every customer leaves not just with a product, but with the confidence that they have the best tool available for their needs and budget.</p>
            </div>
            <div class="info-item">
                <h2>Why Choose Us?</h2>
                <p>We don't just sell; we consult. We analyze your requirements (are you a developer, a content creator, or a casual user?) and provide expert recommendations.</p>
                <p>Our curated selection ensures only reliable brands and tested hardware make it to our shelves, giving you peace of mind that your machine will last.</p>
                </div>
        </div>
    </div>
    <script>
    // Logic to check if user is logged in
    window.onload = function() { 
        if(localStorage.getItem('isLoggedIn') === 'true') { 
            document.getElementById('auth-modal').style.display = 'none';
            document.getElementById('display-email').innerText = localStorage.getItem('userEmail');
        } 
    };

    // Logic to sign in
    function validateAccess() {
        const email = document.getElementById('email').value;
        const pass = document.getElementById('password').value;
        if(email.includes('@') && email.length > 5 && pass.length >= 6) {
            localStorage.setItem('isLoggedIn', 'true');
            localStorage.setItem('userEmail', email);
            document.getElementById('auth-modal').style.display = 'none';
            location.reload();
        } else { 
            alert("Please enter a valid email and a password of at least 6 characters."); 
        }
    }

    // Logic to logout
    function logoutUser() {
        localStorage.removeItem('isLoggedIn');
        localStorage.removeItem('userEmail');
        location.reload();
    }
</script>
</body>
</html>
