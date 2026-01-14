# Loveannivarsary-
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy 7th Anniversary My Love ❤️</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      overflow-x: hidden;
      color: #fff;
    }

    header {
      text-align: center;
      padding: 50px 20px;
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 3.5rem;
      animation: fadeIn 2s ease-in-out;
    }

    h2 {
      margin-top: 10px;
      font-weight: 300;
    }

    .container {
      max-width: 900px;
      margin: auto;
      padding: 20px;
    }

    .card {
      background: rgba(255,255,255,0.15);
      backdrop-filter: blur(6px);
      border-radius: 20px;
      padding: 25px;
      margin: 25px 0;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      animation: slideUp 1.5s ease;
    }

    .card h3 {
      color: #fff;
      margin-bottom: 10px;
    }

    .card p {
      line-height: 1.7;
      font-size: 1.05rem;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
      gap: 15px;
      margin-top: 15px;
    }

    .gallery img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 15px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.3);
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    .love-btn {
      display: block;
      margin: 30px auto;
      padding: 12px 30px;
      border: none;
      border-radius: 30px;
      font-size: 1.1rem;
      cursor: pointer;
      background: #ff4b5c;
      color: #fff;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .love-btn:hover {
      transform: scale(1.08);
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    }

    footer {
      text-align: center;
      padding: 30px 10px;
      font-size: 0.9rem;
      opacity: 0.9;
    }

    /* Heart Animation */
    .heart {
      position: fixed;
      bottom: -20px;
      font-size: 24px;
      animation: floatUp 6s linear infinite;
      opacity: 0.8;
    }

    @keyframes floatUp {
      0% { transform: translateY(0) scale(1); opacity: 1; }
      100% { transform: translateY(-110vh) scale(1.8); opacity: 0; }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    audio {
      display: none;
    }
  </style></head>
<body>  <!-- Background Music (Tap screen once to allow autoplay on mobile) -->  <audio id="bgMusic" loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_5a63b4cfe7.mp3?filename=romantic-piano-112191.mp3" type="audio/mpeg">
  </audio>  <header>
    <h1>Happy 7th Anniversary ❤️</h1>
    <h2>Ritesh & Vaishnavi — Forever Together</h2>
  </header>  <div class="container"><!-- Photo Memories -->
<div class="card">
  <h3>📸 Our Beautiful Memories</h3>
  <p>These smiles, these moments, these memories — they are my biggest treasure. Every photo with you reminds me how lucky I am to love you.</p>
  <div class="gallery">
    <img src="photo1.jpg" alt="Our Memory 1" />
    <img src="photo2.jpg" alt="Our Memory 2" />
  </div>
  <p style="font-size:0.9rem; opacity:0.9;">(Replace <b>photo1.jpg</b> and <b>photo2.jpg</b> with your uploaded photos)</p>
</div>


<div class="card">
  <h3>💖 My Dearest Vaishnavi</h3>
  <p>
    Today is not just another day… it is our beautiful 7th anniversary. 
    Seven years of love, care, memories, fights, smiles, tears, and endless support.
    You are not only my girlfriend, you are my best friend, my happiness, my strength, and my home.
  </p>
</div>

<div class="card">
  <h3>🌸 Our First Meet — 14 June</h3>
  <p>
    I still remember our first meet on <b>14 June</b>. That day changed my life forever.
    Your smile, your voice, and the way you looked at me made my heart feel something magical.
    From that moment, I knew you were special and my life would never be the same again.
  </p>
</div>

<div class="card">
  <h3>🌈 Our Journey Till Today</h3>
  <p>
    From small talks to deep conversations, from silly laughs to emotional moments,
    we have grown together. We learned to understand each other, forgive each other,
    and love each other even more every day. Every memory with you is precious to me.
  </p>
</div>

<div class="card">
  <h3>🤝 My Promise To You</h3>
  <p>
    I promise to always respect you, protect your heart, support your dreams,
    and stand beside you in every situation. No matter what comes in our life,
    I want to walk this beautiful journey with you forever.
  </p>
</div>

<div class="card">
  <h3>💍 My Dream</h3>
  <p>
    I dream of a future where we grow old together, create a happy family,
    and keep loving each other more with every passing year.
    My love for you is endless and pure.
  </p>
</div>

<button class="love-btn" onclick="showLove()">Tap For Love Surprise 💕</button>

  </div><canvas id="fireworks"></canvas>

  <footer>
    Made with infinite love by Ritesh 💖
  </footer>  <script>
    const music = document.getElementById('bgMusic');

    // Start music on first touch (mobile autoplay policy)
    document.body.addEventListener('click', () => {
      music.play().catch(() => {});
    }, { once: true });

    function createHeart() {
      const heart = document.createElement('div');
      heart.classList.add('heart');
      heart.innerHTML = '❤️';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.fontSize = (20 + Math.random() * 30) + 'px';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    setInterval(createHeart, 500);

    function showLove() {
      alert("Vaishnavi ❤️ You are my world. Happy 7th Anniversary! I love you forever. 💕");
      launchFireworks();
    }

    // Fireworks Animation
    const canvas = document.getElementById('fireworks');
    const ctx = canvas.getContext('2d');
    resizeCanvas();
    window.addEventListener('resize', resizeCanvas);

    function resizeCanvas() {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    }

    let particles = [];

    function launchFireworks() {
      for (let i = 0; i < 120; i++) {
        particles.push({
          x: canvas.width / 2,
          y: canvas.height / 2,
          angle: Math.random() * Math.PI * 2,
          speed: Math.random() * 6 + 2,
          radius: Math.random() * 3 + 1,
          life: 100
        });
      }
    }

    function animateFireworks() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);

      particles.forEach((p, index) => {
        const vx = Math.cos(p.angle) * p.speed;
        const vy = Math.sin(p.angle) * p.speed;
        p.x += vx;
        p.y += vy;
        p.life--;

        ctx.beginPath();
        ctx.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
        ctx.fillStyle = 'rgba(255,255,255,0.8)';
        ctx.fill();

        if (p.life <= 0) particles.splice(index, 1);
      });

      requestAnimationFrame(animateFireworks);
    }

    animateFireworks();
  </script></body>
</html><!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy 7th Anniversary My Love ❤️</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      overflow-x: hidden;
      color: #fff;
    }

    header {
      text-align: center;
      padding: 50px 20px;
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 3.5rem;
      animation: fadeIn 2s ease-in-out;
    }

    h2 {
      margin-top: 10px;
      font-weight: 300;
    }

    .container {
      max-width: 900px;
      margin: auto;
      padding: 20px;
    }

    .card {
      background: rgba(255,255,255,0.15);
      backdrop-filter: blur(6px);
      border-radius: 20px;
      padding: 25px;
      margin: 25px 0;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      animation: slideUp 1.5s ease;
    }

    .card h3 {
      color: #fff;
      margin-bottom: 10px;
    }

    .card p {
      line-height: 1.7;
      font-size: 1.05rem;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
      gap: 15px;
      margin-top: 15px;
    }

    .gallery img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 15px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.3);
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    .love-btn {
      display: block;
      margin: 30px auto;
      padding: 12px 30px;
      border: none;
      border-radius: 30px;
      font-size: 1.1rem;
      cursor: pointer;
      background: #ff4b5c;
      color: #fff;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .love-btn:hover {
      transform: scale(1.08);
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    }

    footer {
      text-align: center;
      padding: 30px 10px;
      font-size: 0.9rem;
      opacity: 0.9;
    }

    /* Heart Animation */
    .heart {
      position: fixed;
      bottom: -20px;
      font-size: 24px;
      animation: floatUp 6s linear infinite;
      opacity: 0.8;
    }

    @keyframes floatUp {
      0% { transform: translateY(0) scale(1); opacity: 1; }
      100% { transform: translateY(-110vh) scale(1.8); opacity: 0; }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    audio {
      display: none;
    }
  </style></head>
<body>  <!-- Background Music (Tap screen once to allow autoplay on mobile) -->  <audio id="bgMusic" loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_5a63b4cfe7.mp3?filename=romantic-piano-112191.mp3" type="audio/mpeg">
  </audio>  <header>
    <h1>Happy 7th Anniversary ❤️</h1>
    <h2>Ritesh & Vaishnavi — Forever Together</h2>
  </header>  <div class="container"><!-- Photo Memories -->
<div class="card">
  <h3>📸 Our Beautiful Memories</h3>
  <p>These smiles, these moments, these memories — they are my biggest treasure. Every photo with you reminds me how lucky I am to love you.</p>
  <div class="gallery">
    <img src="photo1.jpg" alt="Our Memory 1" />
    <img src="photo2.jpg" alt="Our Memory 2" />
  </div>
  <p style="font-size:0.9rem; opacity:0.9;">(Replace <b>photo1.jpg</b> and <b>photo2.jpg</b> with your uploaded photos)</p>
</div>


<div class="card">
  <h3>💖 My Dearest Vaishnavi</h3>
  <p>
    Today is not just another day… it is our beautiful 7th anniversary. 
    Seven years of love, care, memories, fights, smiles, tears, and endless support.
    You are not only my girlfriend, you are my best friend, my happiness, my strength, and my home.
  </p>
</div>

<div class="card">
  <h3>🌸 Our First Meet — 14 June</h3>
  <p>
    I still remember our first meet on <b>14 June</b>. That day changed my life forever.
    Your smile, your voice, and the way you looked at me made my heart feel something magical.
    From that moment, I knew you were special and my life would never be the same again.
  </p>
</div>

<div class="card">
  <h3>🌈 Our Journey Till Today</h3>
  <p>
    From small talks to deep conversations, from silly laughs to emotional moments,
    we have grown together. We learned to understand each other, forgive each other,
    and love each other even more every day. Every memory with you is precious to me.
  </p>
</div>

<div class="card">
  <h3>🤝 My Promise To You</h3>
  <p>
    I promise to always respect you, protect your heart, support your dreams,
    and stand beside you in every situation. No matter what comes in our life,
    I want to walk this beautiful journey with you forever.
  </p>
</div>

<div class="card">
  <h3>💍 My Dream</h3>
  <p>
    I dream of a future where we grow old together, create a happy family,
    and keep loving each other more with every passing year.
    My love for you is endless and pure.
  </p>
</div>

<button class="love-btn" onclick="showLove()">Tap For Love Surprise 💕</button>

  </div><canvas id="fireworks"></canvas>

  <footer>
    Made with infinite love by Ritesh 💖
  </footer>  <script>
    const music = document.getElementById('bgMusic');

    // Start music on first touch (mobile autoplay policy)
    document.body.addEventListener('click', () => {
      music.play().catch(() => {});
    }, { once: true });

    function createHeart() {
      const heart = document.createElement('div');
      heart.classList.add('heart');
      heart.innerHTML = '❤️';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.fontSize = (20 + Math.random() * 30) + 'px';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    setInterval(createHeart, 500);

    function showLove() {
      alert("Vaishnavi ❤️ You are my world. Happy 7th Anniversary! I love you forever. 💕");
      launchFireworks();
    }

    // Fireworks Animation
    const canvas = document.getElementById('fireworks');
    const ctx = canvas.getContext('2d');
    resizeCanvas();
    window.addEventListener('resize', resizeCanvas);

    function resizeCanvas() {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    }

    let particles = [];

    function launchFireworks() {
      for (let i = 0; i < 120; i++) {
        particles.push({
          x: canvas.width / 2,
          y: canvas.height / 2,
          angle: Math.random() * Math.PI * 2,
          speed: Math.random() * 6 + 2,
          radius: Math.random() * 3 + 1,
          life: 100
        });
      }
    }

    function animateFireworks() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);

      particles.forEach((p, index) => {
        const vx = Math.cos(p.angle) * p.speed;
        const vy = Math.sin(p.angle) * p.speed;
        p.x += vx;
        p.y += vy;
        p.life--;

        ctx.beginPath();
        ctx.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
        ctx.fillStyle = 'rgba(255,255,255,0.8)';
        ctx.fill();

        if (p.life <= 0) particles.splice(index, 1);
      });

      requestAnimationFrame(animateFireworks);
    }

    animateFireworks();
  </script></body>
</html><!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy 7th Anniversary My Love ❤️</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      overflow-x: hidden;
      color: #fff;
    }

    header {
      text-align: center;
      padding: 50px 20px;
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 3.5rem;
      animation: fadeIn 2s ease-in-out;
    }

    h2 {
      margin-top: 10px;
      font-weight: 300;
    }

    .container {
      max-width: 900px;
      margin: auto;
      padding: 20px;
    }

    .card {
      background: rgba(255,255,255,0.15);
      backdrop-filter: blur(6px);
      border-radius: 20px;
      padding: 25px;
      margin: 25px 0;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      animation: slideUp 1.5s ease;
    }

    .card h3 {
      color: #fff;
      margin-bottom: 10px;
    }

    .card p {
      line-height: 1.7;
      font-size: 1.05rem;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
      gap: 15px;
      margin-top: 15px;
    }

    .gallery img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 15px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.3);
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    .love-btn {
      display: block;
      margin: 30px auto;
      padding: 12px 30px;
      border: none;
      border-radius: 30px;
      font-size: 1.1rem;
      cursor: pointer;
      background: #ff4b5c;
      color: #fff;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .love-btn:hover {
      transform: scale(1.08);
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    }

    footer {
      text-align: center;
      padding: 30px 10px;
      font-size: 0.9rem;
      opacity: 0.9;
    }

    /* Heart Animation */
    .heart {
      position: fixed;
      bottom: -20px;
      font-size: 24px;
      animation: floatUp 6s linear infinite;
      opacity: 0.8;
    }

    @keyframes floatUp {
      0% { transform: translateY(0) scale(1); opacity: 1; }
      100% { transform: translateY(-110vh) scale(1.8); opacity: 0; }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    audio {
      display: none;
    }
  </style></head>
<body>  <!-- Background Music (Tap screen once to allow autoplay on mobile) -->  <audio id="bgMusic" loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_5a63b4cfe7.mp3?filename=romantic-piano-112191.mp3" type="audio/mpeg">
  </audio>  <header>
    <h1>Happy 7th Anniversary ❤️</h1>
    <h2>Ritesh & Vaishnavi — Forever Together</h2>
  </header>  <div class="container"><!-- Photo Memories -->
<div class="card">
  <h3>📸 Our Beautiful Memories</h3>
  <p>These smiles, these moments, these memories — they are my biggest treasure. Every photo with you reminds me how lucky I am to love you.</p>
  <div class="gallery">
    <img src="photo1.jpg" alt="Our Memory 1" />
    <img src="photo2.jpg" alt="Our Memory 2" />
  </div>
  <p style="font-size:0.9rem; opacity:0.9;">(Replace <b>photo1.jpg</b> and <b>photo2.jpg</b> with your uploaded photos)</p>
</div>


<div class="card">
  <h3>💖 My Dearest Vaishnavi</h3>
  <p>
    Today is not just another day… it is our beautiful 7th anniversary. 
    Seven years of love, care, memories, fights, smiles, tears, and endless support.
    You are not only my girlfriend, you are my best friend, my happiness, my strength, and my home.
  </p>
</div>

<div class="card">
  <h3>🌸 Our First Meet — 14 June</h3>
  <p>
    I still remember our first meet on <b>14 June</b>. That day changed my life forever.
    Your smile, your voice, and the way you looked at me made my heart feel something magical.
    From that moment, I knew you were special and my life would never be the same again.
  </p>
</div>

<div class="card">
  <h3>🌈 Our Journey Till Today</h3>
  <p>
    From small talks to deep conversations, from silly laughs to emotional moments,
    we have grown together. We learned to understand each other, forgive each other,
    and love each other even more every day. Every memory with you is precious to me.
  </p>
</div>

<div class="card">
  <h3>🤝 My Promise To You</h3>
  <p>
    I promise to always respect you, protect your heart, support your dreams,
    and stand beside you in every situation. No matter what comes in our life,
    I want to walk this beautiful journey with you forever.
  </p>
</div>

<div class="card">
  <h3>💍 My Dream</h3>
  <p>
    I dream of a future where we grow old together, create a happy family,
    and keep loving each other more with every passing year.
    My love for you is endless and pure.
  </p>
</div>

<button class="love-btn" onclick="showLove()">Tap For Love Surprise 💕</button>

  </div><canvas id="fireworks"></canvas>

  <footer>
    Made with infinite love by Ritesh 💖
  </footer>  <script>
    const music = document.getElementById('bgMusic');

    // Start music on first touch (mobile autoplay policy)
    document.body.addEventListener('click', () => {
      music.play().catch(() => {});
    }, { once: true });

    function createHeart() {
      const heart = document.createElement('div');
      heart.classList.add('heart');
      heart.innerHTML = '❤️';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.fontSize = (20 + Math.random() * 30) + 'px';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    setInterval(createHeart, 500);

    function showLove() {
      alert("Vaishnavi ❤️ You are my world. Happy 7th Anniversary! I love you forever. 💕");
      launchFireworks();
    }

    // Fireworks Animation
    const canvas = document.getElementById('fireworks');
    const ctx = canvas.getContext('2d');
    resizeCanvas();
    window.addEventListener('resize', resizeCanvas);

    function resizeCanvas() {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    }

    let particles = [];

    function launchFireworks() {
      for (let i = 0; i < 120; i++) {
        particles.push({
          x: canvas.width / 2,
          y: canvas.height / 2,
          angle: Math.random() * Math.PI * 2,
          speed: Math.random() * 6 + 2,
          radius: Math.random() * 3 + 1,
          life: 100
        });
      }
    }

    function animateFireworks() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);

      particles.forEach((p, index) => {
        const vx = Math.cos(p.angle) * p.speed;
        const vy = Math.sin(p.angle) * p.speed;
        p.x += vx;
        p.y += vy;
        p.life--;

        ctx.beginPath();
        ctx.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
        ctx.fillStyle = 'rgba(255,255,255,0.8)';
        ctx.fill();

        if (p.life <= 0) particles.splice(index, 1);
      });

      requestAnimationFrame(animateFireworks);
    }

    animateFireworks();
  </script></body>
</html><!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy 7th Anniversary My Love ❤️</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      overflow-x: hidden;
      color: #fff;
    }

    header {
      text-align: center;
      padding: 50px 20px;
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 3.5rem;
      animation: fadeIn 2s ease-in-out;
    }

    h2 {
      margin-top: 10px;
      font-weight: 300;
    }

    .container {
      max-width: 900px;
      margin: auto;
      padding: 20px;
    }

    .card {
      background: rgba(255,255,255,0.15);
      backdrop-filter: blur(6px);
      border-radius: 20px;
      padding: 25px;
      margin: 25px 0;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      animation: slideUp 1.5s ease;
    }

    .card h3 {
      color: #fff;
      margin-bottom: 10px;
    }

    .card p {
      line-height: 1.7;
      font-size: 1.05rem;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
      gap: 15px;
      margin-top: 15px;
    }

    .gallery img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 15px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.3);
      transition: transform 0.3s;
    }

    .gallery img:hover {
      transform: scale(1.05);
    }

    .love-btn {
      display: block;
      margin: 30px auto;
      padding: 12px 30px;
      border: none;
      border-radius: 30px;
      font-size: 1.1rem;
      cursor: pointer;
      background: #ff4b5c;
      color: #fff;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .love-btn:hover {
      transform: scale(1.08);
      box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    }

    footer {
      text-align: center;
      padding: 30px 10px;
      font-size: 0.9rem;
      opacity: 0.9;
    }

    /* Heart Animation */
    .heart {
      position: fixed;
      bottom: -20px;
      font-size: 24px;
      animation: floatUp 6s linear infinite;
      opacity: 0.8;
    }

    @keyframes floatUp {
      0% { transform: translateY(0) scale(1); opacity: 1; }
      100% { transform: translateY(-110vh) scale(1.8); opacity: 0; }
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes slideUp {
      from { opacity: 0; transform: translateY(40px); }
      to { opacity: 1; transform: translateY(0); }
    }

    audio {
      display: none;
    }
  </style></head>
<body>  <!-- Background Music (Tap screen once to allow autoplay on mobile) -->  <audio id="bgMusic" loop>
    <source src="https://cdn.pixabay.com/download/audio/2022/03/15/audio_5a63b4cfe7.mp3?filename=romantic-piano-112191.mp3" type="audio/mpeg">
  </audio>  <header>
    <h1>Happy 7th Anniversary ❤️</h1>
    <h2>Ritesh & Vaishnavi — Forever Together</h2>
  </header>  <div class="container"><!-- Photo Memories -->
<div class="card">
  <h3>📸 Our Beautiful Memories</h3>
  <p>These smiles, these moments, these memories — they are my biggest treasure. Every photo with you reminds me how lucky I am to love you.</p>
  <div class="gallery">
    <img src="photo1.jpg" alt="Our Memory 1" />
    <img src="photo2.jpg" alt="Our Memory 2" />
  </div>
  <p style="font-size:0.9rem; opacity:0.9;">(Replace <b>photo1.jpg</b> and <b>photo2.jpg</b> with your uploaded photos)</p>
</div>


<div class="card">
  <h3>💖 My Dearest Vaishnavi</h3>
  <p>
    Today is not just another day… it is our beautiful 7th anniversary. 
    Seven years of love, care, memories, fights, smiles, tears, and endless support.
    You are not only my girlfriend, you are my best friend, my happiness, my strength, and my home.
  </p>
</div>

<div class="card">
  <h3>🌸 Our First Meet — 14 June</h3>
  <p>
    I still remember our first meet on <b>14 June</b>. That day changed my life forever.
    Your smile, your voice, and the way you looked at me made my heart feel something magical.
    From that moment, I knew you were special and my life would never be the same again.
  </p>
</div>

<div class="card">
  <h3>🌈 Our Journey Till Today</h3>
  <p>
    From small talks to deep conversations, from silly laughs to emotional moments,
    we have grown together. We learned to understand each other, forgive each other,
    and love each other even more every day. Every memory with you is precious to me.
  </p>
</div>

<div class="card">
  <h3>🤝 My Promise To You</h3>
  <p>
    I promise to always respect you, protect your heart, support your dreams,
    and stand beside you in every situation. No matter what comes in our life,
    I want to walk this beautiful journey with you forever.
  </p>
</div>

<div class="card">
  <h3>💍 My Dream</h3>
  <p>
    I dream of a future where we grow old together, create a happy family,
    and keep loving each other more with every passing year.
    My love for you is endless and pure.
  </p>
</div>

<button class="love-btn" onclick="showLove()">Tap For Love Surprise 💕</button>

  </div><canvas id="fireworks"></canvas>

  <footer>
    Made with infinite love by Ritesh 💖
  </footer>  <script>
    const music = document.getElementById('bgMusic');

    // Start music on first touch (mobile autoplay policy)
    document.body.addEventListener('click', () => {
      music.play().catch(() => {});
    }, { once: true });

    function createHeart() {
      const heart = document.createElement('div');
      heart.classList.add('heart');
      heart.innerHTML = '❤️';
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.fontSize = (20 + Math.random() * 30) + 'px';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    setInterval(createHeart, 500);

    function showLove() {
      alert("Vaishnavi ❤️ You are my world. Happy 7th Anniversary! I love you forever. 💕");
      launchFireworks();
    }

    // Fireworks Animation
    const canvas = document.getElementById('fireworks');
    const ctx = canvas.getContext('2d');
    resizeCanvas();
    window.addEventListener('resize', resizeCanvas);

    function resizeCanvas() {
      canvas.width = window.innerWidth;
      canvas.height = window.innerHeight;
    }

    let particles = [];

    function launchFireworks() {
      for (let i = 0; i < 120; i++) {
        particles.push({
          x: canvas.width / 2,
          y: canvas.height / 2,
          angle: Math.random() * Math.PI * 2,
          speed: Math.random() * 6 + 2,
          radius: Math.random() * 3 + 1,
          life: 100
        });
      }
    }

    function animateFireworks() {
      ctx.clearRect(0, 0, canvas.width, canvas.height);

      particles.forEach((p, index) => {
        const vx = Math.cos(p.angle) * p.speed;
        const vy = Math.sin(p.angle) * p.speed;
        p.x += vx;
        p.y += vy;
        p.life--;

        ctx.beginPath();
        ctx.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
        ctx.fillStyle = 'rgba(255,255,255,0.8)';
²        ctx.fill();

        if (p.life <= 0) particles.splice(index, 1);
      });

      requestAnimationFrame(animateFireworks);
    }

    animateFireworks();
  </script></b
