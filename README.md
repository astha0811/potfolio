
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Astha's Portfolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    .typing-text {
  font-weight: bold;
  font-size: 18px;
  color: var(--accent);
}

.cursor {
  display: inline-block;
  animation: blink 0.8s infinite;
  font-weight: bold;
  font-size: 20px;
}

@keyframes blink {
  0%, 100% { opacity: 1; }
  50% { opacity: 0; }
}

    :root {
    body::before {
  content: "";
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: url('https://images.unsplash.com/photo-1575467544611-470fa8053545?w=600&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1yZWxhdGVkfDYzfHx8ZW58MHx8fHx8') no-repeat center center/cover;
  filter: brightness(0.7) blur(4px);
  z-index: -1;
  opacity: 0.9;
    }

      --bg-light: #f4f4f4;
      --bg-dark: #121212;
      --text-light: #000;
      --text-dark: #fff;
      --accent: #0e5576;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      transition: background 0.4s, color 0.4s;
    }

    body.light {
      background: var(--bg-light);
      color: var(--text-light);
    }

    body.dark {
      background: var(--bg-dark);
      color: var(--text-dark);
    }

    header {
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: var(--accent);
    }

    header h1 {
      margin: 0;
      font-size: 26px;
      color: #fff;
    }

    nav a {
      margin: 0 10px;
      color: #fff;
      text-decoration: none;
      font-weight: bold;
    }

  
      .container {
  padding: 2rem;
  max-width: 1000px;
  margin: auto;
  background: rgba(255, 255, 255, 0.2);
  border-radius: 16px;
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  box-shadow: 0 4px 30px rgba(0, 0, 0, 0.2);
}

    

    section {
      margin: 4rem 0;
      opacity: 0;
      transform: translateY(20px);
      animation: fadeIn 0.8s ease forwards;
    }

    section:nth-of-type(1) { animation-delay: 0.4s; }
    section:nth-of-type(2) { animation-delay: 0.6s; }
    section:nth-of-type(3) { animation-delay: 0.8s; }
    section:nth-of-type(4) { animation-delay: 0.10s; }

    @keyframes fadeIn {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    h2 {
      border-bottom: 2px solid var(--accent);
      padding-bottom: 0.5rem;
    }

    .about-section {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 2rem;
    }

    .about-img {
  flex: 1 1 200px;
  max-width: 250px;
  width: 100%;
  height: auto;
  border-radius: 30x; 
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2); 
}

    

    .about-text {
      flex: 2;
    }

    .skills-list {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .skills-list span {
      background: var(--accent);
      padding: 6px 12px;
      border-radius: 20px;
      color: #fff;
      font-size: 14px;
    }

    .projects-grid {
      display: grid;
      gap: 1rem;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    }

    .project-card {
      border: 1px solid #ccc;
      border-radius: 10px;
      padding: 1rem;
      background: #fff;
      color: #000;
      transition: transform 0.3s;
    }

    .project-card:hover {
      transform: translateY(-5px);
    }

    .dark .project-card {
      background: #1f1f1f;
      color: #fff;
      border-color: #444;
    }

    .contact-form input, .contact-form textarea {
      width: 100%;
      padding: 8px;
      margin: 0.5rem 0;
      border-radius: 8px;
      border: 1px solid #ccc;
    }

    .contact-form button {
      background: var(--accent);
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    footer {
      text-align: center;
      padding: 1rem;
      background: var(--accent);
      color: #fff;
    }

    .theme-toggle {
      background: #fff;
      border: none;
      padding: 5px 12px;
      border-radius: 20px;
      font-weight: bold;
      cursor: pointer;
    }

    @media (max-width: 600px) {
      .about-section {
        flex-direction: column;
        text-align: center;
      }
    }
  </style>
</head>
<body class="light">
  <header>
    <h1>Astha Keshari</h1>
    <nav>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
      <button class="theme-toggle" onclick="toggleTheme()">🌙</button>
    </nav>
  </header>

  <div class="container">
    <section id="about">
      <h2>About Me</h2>
      <div class="about-section">
        <img src="https://i.postimg.cc/4NyJhMB1/Whats-App-Image-2025-07-19-at-23-16-30-0b90437b.jpg" alt="My Photo" class="about-img" />
        <div class="about-text">
          <h3>Hello! I'm <strong>Astha</strong></h3>
<p><span class="typing-text"></span><span class="cursor">|</span></p>

          <p>🎓 <strong>College:</strong> Indian Institute of Information technology Ranchi</p>
          <p>📅 <strong>Year:</strong> First Year</p>
          <p>📚 <strong>Branch:</strong> Computer Science and Engineering</p>
          <p>I love building creative web apps, and I'm constantly learning new technologies to improve myself.</p>
        </div>
      </div>
    </section>

    <section id="skills">
      <h2>Skills</h2>
      <div class="skills-list">
        <span>HTML</span>
        <span>CSS</span>
        <span>JavaScript</span>
        <span>Bootstrap</span>
        <span>C++</span>
        <span>Git & GitHub</span>
        <span>Responsive Design</span>
      </div>
    </section>

    <section id="projects">
      <h2>Projects</h2>
      <div class="projects-grid">
        <div class="project-card">
          <h3>🌤 Weather App</h3>
          <p>Responsive weather app using API, emojis, dark/light mode, and modern UI.</p>
          

        </div>
        <div class="project-card">
          <h3>✅ To-Do List</h3>
          <p>A smart task manager using JavaScript and local storage with sleek design.</p>
          <li><a href="todo.html">To-Do</a></li>

        </div>
        <div class="project-card">
          <h3>🎨 Personal Portfolio</h3>
          <p>This very portfolio! Made with love, design thinking, and animations.</p>
        </div>
      </div>
    </section>

    <section id="contact">
      <h2>Contact Me</h2>
      <form class="contact-form">
        <input type="text" placeholder="Your Name" required />
        <input type="email" placeholder="Your Email" required />
        <textarea rows="4" placeholder="Your Message"></textarea>
        <button type="submit">Send</button>
      </form>
      <div style="text-align: center; margin-top: 20px;">
  <h3>Connect with me</h3>
  <a href="https://www.linkedin.com/in/asthakeshari" target="_blank" style="margin: 0 10px; color: #0e76a8;">
    <i class="fab fa-linkedin fa-2x"></i>
  </a>
  <a href="https://github.com/astha0811" target="_blank" style="margin: 0 10px; color: #333;">
    <i class="fab fa-github fa-2x"></i>
  </a>
  <a href="https://www.instagram.com/_____astha.__" target="_blank" style="margin: 0 10px; color: #C13584;">
    <i class="fab fa-instagram fa-2x"></i>
  </a>
  <a href="mailto:aasthakeshari0@gmail.com" style="margin: 0 15px; color: #EA4335;">
    <i class="fas fa-envelope fa-2x"></i>
  </a>
</div>

    </section>
  </div>

  <footer>
    <p>&copy; 2025 Astha Keshari • Built with 💖</p>
  </footer>

  <script>
    function toggleTheme() {
      const body = document.body;
      body.classList.toggle('dark');
      body.classList.toggle('light');
      document.querySelector('.theme-toggle').textContent =
        body.classList.contains('dark') ? '☀️' : '🌙';
    }
  </script>
  <script>
  const textArray = [
    "a Web Developer",
    "a Designer",
    "a Creative Thinker",
    "a Problem Solver"
  ];
  const typingText = document.querySelector(".typing-text");
  let textIndex = 0;
  let charIndex = 0;
  let isDeleting = false;

  function type() {
    const currentText = textArray[textIndex];
    if (isDeleting) {
      typingText.textContent = currentText.substring(0, charIndex--);
    } else {
      typingText.textContent = currentText.substring(0, charIndex++);
    }

    if (!isDeleting && charIndex === currentText.length) {
      isDeleting = true;
      setTimeout(type, 1000);
    } else if (isDeleting && charIndex === 0) {
      isDeleting = false;
      textIndex = (textIndex + 1) % textArray.length;
      setTimeout(type, 300);
    } else {
      setTimeout(type, isDeleting ? 50 : 100);
    }
  }

  type();
</script>

</body>
</html>   
