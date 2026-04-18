<header>
  <h1 class="logo-text">TIM-2 RACING</h1>
  <p class="subtitle">Driven to win</p>

  <button onclick="scrollToSection('about')">О команде</button>
  <button onclick="scrollToSection('contact')">Контакты</button>
</header>

<section id="about" class="fade">
  <h2>О команде</h2>
  <p>Мы — TIM-2 Racing. Молодая гоночная команда с амбициями выйти на топ уровень.</p>
</section>

<section id="contact" class="fade">
  <h2>Контакты</h2>
  <p>TikTok / YouTube скоро 🚀</p>
</section>

<footer>
  <p>© TIM-2 RACING</p>
</footer>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #0b0f1a;
  color: white;
  scroll-behavior: smooth;
}

header {
  text-align: center;
  padding: 60px 20px;
  background: linear-gradient(90deg, #0b0f1a, #1e6bff);
}

.logo-img {
  width: 120px;
  margin-bottom: 10px;
  animation: fadeIn 1.5s ease;
}

.logo-text {
  font-size: 40px;
  transform: skew(-10deg);
  animation: fadeIn 2s ease;
}

.subtitle {
  opacity: 0.8;
  margin-bottom: 20px;
  animation: fadeIn 2.5s ease;
}

button {
  margin: 5px;
  padding: 10px 20px;
  background: #1e6bff;
  border: none;
  color: white;
  cursor: pointer;
  transition: 0.3s;
}

button:hover {
  background: white;
  color: black;
  transform: scale(1.1);
}

section {
  padding: 60px 20px;
  text-align: center;
}

footer {
  padding: 20px;
  text-align: center;
  background: #111;
}

/* АНИМАЦИИ */
.fade {
  opacity: 0;
  transform: translateY(40px);
  transition: all 1s ease;
}

.fade.show {
  opacity: 1;
  transform: translateY(0);
}

@keyframes fadeIn {
  from {opacity: 0;}
  to {opacity: 1;}
}