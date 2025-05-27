<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Jozef Hosting</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Jozef Hosting</h1>
    <nav>
      <ul>
        <li><a href="#pricing">Pricing</a></li>
        <li><a href="#buy-ticket">Buy Ticket</a></li>
        <li><a href="#features">Features</a></li>
      </ul>
    </nav>
  </header>

  <section id="pricing">
    <h2>Our Hosting Plans</h2>
    <div class="plans">
      <div class="plan">
        <h3>Basic</h3>
        <p class="price">$5 / month</p>
        <p>10 GB Storage, 100 GB Bandwidth</p>
      </div>
      <div class="plan">
        <h3>Standard</h3>
        <p class="price">$10 / month</p>
        <p>50 GB Storage, 500 GB Bandwidth</p>
      </div>
      <div class="plan">
        <h3>Premium</h3>
        <p class="price">$20 / month</p>
        <p>Unlimited Storage, Unlimited Bandwidth</p>
      </div>
    </div>
  </section>

  <section id="buy-ticket">
    <h2>Buy Your Hosting Ticket</h2>
    <button class="buy-btn">Buy Now</button>
  </section>

  <section id="features">
    <h2>Why Choose Jozef Hosting?</h2>
    <ul>
      <li>99.9% Uptime Guarantee</li>
      <li>24/7 Customer Support</li>
      <li>Fast & Secure Servers</li>
      <li>Easy Setup & Management</li>
    </ul>
  </section>

  <footer>
    <p>&copy; 2025 Jozef Hosting. All rights reserved.</p>
  </footer>
</body>
</html>

<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Jozef Hosting with Discord & Ticket</title>
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet" />
<style>
  /* Basic reset */
  * {
    margin: 0; padding: 0; box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }
  body {
    background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
    color: #00ff80;
    min-height: 100vh;
    display: flex;
  }

  /* Sidebar Discord info */
  #discord-sidebar {
    position: fixed;
    left: 0; top: 0; bottom: 0;
    width: 250px;
    background: rgba(0,255,128,0.1);
    border-right: 2px solid #00ff80;
    box-shadow: 0 0 20px #00ff80;
    padding: 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  #discord-sidebar h2 {
    color: #00ff80;
    text-shadow: 0 0 10px #00ff80;
    font-weight: 900;
    margin-bottom: 20px;
  }
  #discord-sidebar p {
    font-size: 0.9rem;
    margin-bottom: 10px;
    color: #a3f7bf;
  }
  #discord-sidebar a {
    display: block;
    text-align: center;
    margin-top: 20px;
    padding: 12px 0;
    background: #00ff80;
    color: #022;
    font-weight: 700;
    border-radius: 25px;
    text-decoration: none;
    box-shadow: 0 0 15px #00ff80;
    transition: background 0.3s ease, box-shadow 0.3s ease;
  }
  #discord-sidebar a:hover {
    background: #00cc66;
    box-shadow: 0 0 25px #00cc66;
  }

  /* Main content */
  main {
    margin-left: 250px;
    padding: 40px 30px;
    flex: 1;
  }

  /* Neon flicker effect on titles */
  .neon-title {
    font-size: 3rem;
    font-weight: 900;
    color: #00ff80;
    text-shadow:
      0 0 5px #00ff80,
      0 0 15px #00ff80,
      0 0 30px #00ff80,
      0 0 60px #00ff80;
    animation: flicker 3s infinite;
  }

  @keyframes flicker {
    0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% {
      text-shadow:
        0 0 5px #00ff80,
        0 0 15px #00ff80,
        0 0 30px #00ff80,
        0 0 60px #00ff80;
    }
    20%, 22%, 24%, 55% {
      text-shadow: none;
      color: #0f2027;
    }
  }

  /* Form styles */
  form {
    max-width: 500px;
    background: rgba(0,255,128,0.15);
    border-radius: 15px;
    padding: 25px 30px;
    box-shadow: 0 0 20px #00ff80cc;
  }
  form label {
    display: block;
    font-weight: 700;
    margin-bottom: 8px;
    color: #00ff80;
  }
  form input, form select {
    width: 100%;
    padding: 10px;
    border-radius: 8px;
    border: none;
    margin-bottom: 15px;
    font-size: 1rem;
    font-weight: 600;
    color: #022;
  }
  form button {
    background: #00ff80;
    color: #022;
    font-weight: 900;
    font-size: 1.2rem;
    padding: 12px;
    border: none;
    border-radius: 25px;
    cursor: pointer;
    box-shadow: 0 0 20px #00ff80cc;
    transition: background 0.3s ease, box-shadow 0.3s ease;
  }
  form button:hover {
    background: #00cc66;
    box-shadow: 0 0 30px #00cc66;
  }

  /* Validation message */
  .error {
    color: #ff4444;
    font-size: 0.9rem;
    margin-bottom: 10px;
  }
</style>
</head>
<body>

  <aside id="discord-sidebar">
    <h2>Discord Info</h2>
    <p><i class="fa-brands fa-discord"></i> Username: <b>Jozef#1234</b></p>
    <p>Status: <span style="color: #0f0;">Online</span></p>
    <a href="https://discord.gg/your-invite" target="_blank" rel="noopener">Contact me on Discord</a>
  </aside>

  <main>
    <h1 class="neon-title">Jozef Hosting - Order Ticket</h1>

    <form id="orderForm" novalidate>
      <label for="plan">Select Hosting Plan</label>
      <select id="plan" name="plan" required>
        <option value="">-- Choose a plan --</option>
        <option value="basic">Basic - $5/mo</option>
        <option value="standard">Standard - $10/mo</option>
        <option value="premium">Premium - $20/mo</option>
      </select>

      <label for="email">Email</label>
      <input type="email" id="email" name="email" placeholder="example@mail.com" required />

      <label for="phone">Phone Number</label>
      <input type="tel" id="phone" name="phone" placeholder="+1234567890" pattern="^\+?\d{7,15}$" required />

      <label for="captcha">Verify you're human: 2 + 3 = ?</label>
      <input type="number" id="captcha" name="captcha" placeholder="Answer here" required />

      <div class="error" id="errorMsg"></div>

      <button type="submit">Submit Order</button>
    </form>
  </main>

<script>
  const form = document.getElementById('orderForm');
  const errorMsg = document.getElementById('errorMsg');

  form.addEventListener('submit', e => {
    e.preventDefault();
    errorMsg.textContent = '';

    const plan = form.plan.value;
    const email = form.email.value.trim();
    const phone = form.phone.value.trim();
    const captcha = form.captcha.value.trim();

    if (!plan) {
      errorMsg.textContent = 'Please select a hosting plan.';
      return;
    }
    if (!email || !validateEmail(email)) {
      errorMsg.textContent = 'Please enter a valid email.';
      return;
    }
    if (!phone || !validatePhone(phone)) {
      errorMsg.textContent = 'Please enter a valid phone number.';
      return;
    }
    if (captcha !== '5') {
      errorMsg.textContent = 'Captcha answer is incorrect.';
      return;
    }

    alert(`Order submitted!\nPlan: ${plan}\nEmail: ${email}\nPhone: ${phone}`);
    form.reset();
  });

  function validateEmail(email) {
    // simple email regex
    return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
  }
  function validatePhone(phone) {
    // matches digits and optional leading +
    return /^\+?\d{7,15}$/.test(phone);
  }
</script>

</body>
</html>
/* Reset & base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  scroll-behavior: smooth;
  transition: all 0.3s ease;
  user-select: none;
}

body {
  background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
  color: #e0f7fa;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

/* Header */
header {
  padding: 1.5rem 3rem;
  background: rgba(0, 255, 128, 0.1);
  display: flex;
  justify-content: space-between;
  align-items: center;
  backdrop-filter: blur(8px);
  border-bottom: 1px solid #00ff80aa;
}

header h1 {
  font-size: 2.2rem;
  color: #00ff80;
  text-shadow: 0 0 8px #00ff80;
}

nav ul {
  list-style: none;
  display: flex;
  gap: 2rem;
}

nav a {
  text-decoration: none;
  color: #a3f7bf;
  font-weight: 600;
  position: relative;
}

nav a::after {
  content: '';
  position: absolute;
  bottom: -6px;
  left: 0;
  width: 0;
  height: 3px;
  background: #00ff80;
  border-radius: 2px;
  transition: width 0.3s ease;
}

nav a:hover::after {
  width: 100%;
}

/* Pricing Section */
#pricing {
  padding: 3rem 2rem;
  text-align: center;
  background: rgba(0, 255, 128, 0.05);
  margin: 2rem auto;
  max-width: 900px;
  border-radius: 12px;
  box-shadow: 0 0 18px #00ff80aa;
}

#pricing h2 {
  font-size: 2rem;
  margin-bottom: 2rem;
  color: #00ff80;
  text-shadow: 0 0 5px #00ff80;
}

.plans {
  display: flex;
  gap: 1.5rem;
  justify-content: center;
  flex-wrap: wrap;
}

.plan {
  background: rgba(0, 255, 128, 0.15);
  border-radius: 12px;
  padding: 1.8rem 1.5rem;
  width: 250px;
  box-shadow: 0 0 10px #00ff80cc;
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.plan:hover {
  transform: scale(1.07);
  box-shadow: 0 0 20px #00ff80ff;
}

.plan h3 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #00ff80;
}

.price {
  font-size: 1.3rem;
  margin-bottom: 1rem;
  font-weight: bold;
  color: #00ff80;
}

/* Buy Ticket */
#buy-ticket {
  padding: 2rem;
  background: rgba(0, 255, 128, 0.1);
  text-align: center;
  margin: 2rem auto;
  max-width: 500px;
  border-radius: 12px;
  box-shadow: 0 0 15px #00ff80aa;
}

.buy-btn {
  background: #00ff80;
  color: #022;
  font-weight: 700;
  font-size: 1.4rem;
  padding: 0.8rem 2.2rem;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  box-shadow: 0 0 12px #00ff80dd;
  transition: background 0.3s ease;
}

.buy-btn:hover {
  background: #00cc66;
  box-shadow: 0 0 20px #00cc66ff;
}

/* Features */
#features {
  padding: 3rem 2rem;
  background: rgba(0, 255, 128, 0.05);
  margin: 2rem auto 3rem;
  max-width: 700px;
  border-radius: 12px;
  box-shadow: 0 0 18px #00ff80aa;
}

#features h2 {
  color: #00ff80;
  margin-bottom: 1.5rem;
  text-align: center;
  font-size: 2rem;
  text-shadow: 0 0 8px #00ff80;
}

#features ul {
  list-style: none;
  color: #a3f7bf;
  font-weight: 600;
  font-size: 1.2rem;
  display: grid;
  gap: 1rem;
  max-width: 400px;
  margin: 0 auto;
}

/* Footer */
footer {
  background: #022;
  color: #00ff80;
  padding: 1rem;
  text-align: center;
  font-size: 0.9rem;
  border-top: 1px solid #00ff80aa;
  box-shadow: 0 0 10px #00ff80cc inset;
}

