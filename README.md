<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Praneetha Sripada | Portfolio</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <style>
    :root {
      --bg: #fdf7ff;
      --bg-alt: #f4f0ff;
      --accent: #7c3aed;     /* soft violet */
      --accent-soft: #e9ddff;
      --pill1: #ffe4e6;      /* pastel pink */
      --pill2: #dbeafe;      /* pastel blue */
      --pill3: #dcfce7;      /* pastel green */
      --pill4: #fee2ff;      /* pastel purple */
      --text-main: #1f2933;
      --text-muted: #6b7280;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: radial-gradient(circle at top left, #fef3ff, #fdf7ff 45%, #e0f2fe 100%);
      color: var(--text-main);
      line-height: 1.6;
    }

    a { color: var(--accent); text-decoration: none; }

    header {
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(12px);
      background: rgba(253,247,255,0.86);
      border-bottom: 1px solid #e5e7eb;
    }

    .nav {
      max-width: 960px;
      margin: 0 auto;
      padding: 0.75rem 1rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .nav-brand {
      font-weight: 800;
      letter-spacing: 0.08em;
      font-size: 0.95rem;
      color: var(--accent);
      text-transform: uppercase;
    }

    .nav-links a {
      margin-left: 1.25rem;
      font-size: 0.9rem;
      color: var(--text-muted);
    }

    main {
      max-width: 960px;
      margin: 0 auto;
      padding: 1.5rem 1rem 3rem;
    }

    section { padding: 4rem 0 1rem; }

    h1, h2, h3 { font-weight: 700; }

    h1 { font-size: 2.3rem; margin-bottom: 0.75rem; }

    h2 {
      font-size: 1.6rem;
      margin-bottom: 1rem;
      padding-bottom: 0.4rem;
      border-bottom: 2px solid var(--accent-soft);
    }

    p { margin-bottom: 0.75rem; }

    .muted { color: var(--text-muted); font-size: 0.96rem; }

    /* hero */
    .hero {
      min-height: 60vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .hero-tag {
      text-transform: uppercase;
      font-size: 0.75rem;
      color: var(--accent);
      letter-spacing: 0.18em;
      margin-bottom: 0.5rem;
    }

    .hero-actions {
      margin-top: 1.25rem;
      display: flex;
      gap: 0.75rem;
      flex-wrap: wrap;
    }

    .btn {
      padding: 0.55rem 1.1rem;
      border-radius: 999px;
      border: 1px solid var(--accent);
      font-size: 0.9rem;
      cursor: pointer;
      background: white;
      color: var(--accent);
      box-shadow: 0 8px 18px rgba(124,58,237,0.12);
    }

    .btn-primary {
      background: var(--accent);
      color: white;
      border-color: transparent;
    }

    /* layout helpers */
    .grid-2 {
      display: grid;
      grid-template-columns: minmax(0, 1.4fr) minmax(0, 1fr);
      gap: 1.75rem;
    }

    .card {
      background: var(--bg-alt);
      border-radius: 1rem;
      padding: 1.25rem 1.3rem;
      border: 1px solid #e5e7eb;
      box-shadow: 0 10px 25px rgba(148,163,184,0.14);
    }

    ul { padding-left: 1.15rem; }
    li { margin-bottom: 0.35rem; }

    /* pastel tech pills */
    .pill {
      display: inline-flex;
      align-items: center;
      padding: 0.22rem 0.7rem;
      border-radius: 999px;
      font-size: 0.8rem;
      font-weight: 500;
      margin: 0 0.4rem 0.4rem 0;
      color: #111827;
      border: 1px solid rgba(148,163,184,0.4);
    }

    .pill.p1 { background: var(--pill1); }
    .pill.p2 { background: var(--pill2); }
    .pill.p3 { background: var(--pill3); }
    .pill.p4 { background: var(--pill4); }

    /* project tiles */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1.5rem;
    }

    .project-card {
      background: white;
      border-radius: 1rem;
      padding: 1.1rem 1.2rem;
      border: 1px solid #e5e7eb;
      box-shadow: 0 10px 26px rgba(148,163,184,0.18);
      position: relative;
      overflow: hidden;
    }

    .project-tag {
      font-size: 0.75rem;
      color: var(--text-muted);
      margin-bottom: 0.4rem;
    }

    .project-lang {
      position: absolute;
      top: 0.8rem;
      right: 0.9rem;
    }

    @media (max-width: 720px) {
      .grid-2 { grid-template-columns: minmax(0, 1fr); }
      h1 { font-size: 1.9rem; }
      .nav-links { font-size: 0.9rem; }
      .nav-links a { margin-left: 0.75rem; }
    }
  </style>
</head>
<body>
<header>
  <div class="nav">
    <div class="nav-brand">PRANEETHA</div>
    <div class="nav-links">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</header>

<main>
  <!-- Hero / Home -->
  <section id="home" class="hero">
    <span class="hero-tag">Full Stack Developer </span>
    <h1>Building clean, practical solutions with code.</h1>
    <p class="muted">
     I am a passionate Python full-stack developer in progress, focused on building clean, user-friendly applications. 
     With a strong problem-solving mindset and attention to detail, I love turning ideas into functional and 
     meaningful digital experiences.
    </p>
    <div class="hero-actions">
      <a href="#projects" class="btn btn-primary">View Projects</a>
      <a href="#contact" class="btn">Let’s connect</a>
     <a href="https://github.com/Praneetha-coder/raw/main/Praneetha's%20Resume-hackerresume%20(3).pdf" class="btn" target="_blank" rel="noopener">
  View Resume
      </a>
    </div>
  </section>

  <!-- About -->
  <section id="about">
    <h2>About</h2>
    <div class="grid-2">
  <div>
    <p>
      I'm <strong>Praneetha Sripada</strong>, an aspiring Python full-stack developer with hands-on experience
      in web development, data science, and GenAI workflows. I enjoy building clean, user-friendly
      applications while continuously improving my skills in frontend, backend, and problem-solving.
      I'm passionate about creating practical solutions, collaborating with teams, and writing code
      that is both efficient and reliable.
    </p>
  </div>
</div>

      <div class="card">
        <h3>Snapshot</h3>
        <ul>
          <li>B.Tech in Information Technology, BVRIT Hyderabad (2021–2025).</li>
          <li>Strong foundation in Python, SQL, HTML, CSS, and JavaScript, with ongoing learning in React and backend development.</li>
          <li>Experience working on real-world academic and self-driven projects, including ML-based and full-stack applications.</li>
          <li>Quick learner with strong communication skills and the ability to explain technical concepts clearly.</li>
          <li>Dedicated to writing clean, maintainable code and continuously improving my development skills.</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- Skills with pastel boxes -->
  <section id="skills">
    <h2>Skills</h2>
    <div class="card">
      <h3>Programming Languages</h3>
      <p>
        <span class="pill p1">Python</span>
        <span class="pill p2">JavaScript</span>
        <span class="pill p3">SQL</span>
        <span class="pill p4">HTML</span>
        <span class="pill p2">CSS</span>
      </p>

      <h3>Frameworks & Libraries</h3>
      <p>
        <span class="pill p2">React (learning)</span>
        <span class="pill p1">Bootstrap</span>
        <span class="pill p4">Tailwind CSS</span>
        <span class="pill p3">Flask (learning)</span>
      </p>

      <h3>Tools & Platforms</h3>
      <p>
        <span class="pill p2">Git & GitHub</span>
        <span class="pill p1">VS Code</span>
        <span class="pill p3">Google Colab</span>
      </p>
    </div>
  </section>

  <!-- Projects with pastel language boxes -->
  <section id="projects">
    <h2>Projects</h2>
    <div class="projects-grid">

      <div class="project-card">
        <div class="project-lang">
          <span class="pill p2">Python</span>
        </div>
        <h3>Driver Drowsiness Detection</h3>
        <p class="project-tag">Python · Keras · TensorFlow · Computer Vision</p>
        <p>
          CNN‑based system that monitors eye patterns from video frames and raises alerts
          when signs of drowsiness are detected.
        </p>
        <!-- <a href="YOUR_GITHUB_LINK" target="_blank">View code →</a> -->
      </div>

      <div class="project-card">
        <div class="project-lang">
          <span class="pill p3">Arduino</span>
        </div>
        <h3>Arduino Fire‑Fighting Robot</h3>
        <p class="project-tag">Arduino · Flame Sensors · GSM · Embedded C/C++</p>
        <p>
          Autonomous robot that detects fire using flame and temperature sensors,
          navigates via ultrasonic sensors, and activates a water pump while sending GSM alerts.
        </p>
      </div>

      <div class="project-card">
        <div class="project-lang">
          <span class="pill p4">IoT</span>
        </div>
        <h3>AI‑IoT Smart Stove</h3>
        <p class="project-tag">IoT · Gas Sensors · Basic ML</p>
        <p>
          Safety‑focused stove prototype with gas‑leak detection, automatic shutdown,
          and mobile‑style real‑time notifications.
        </p>
      </div>

      <div class="project-card">
        <div class="project-lang">
          <span class="pill p1">Python</span>
        </div>
        <h3>Hangman Game</h3>
        <p class="project-tag">Python · Tkinter</p>
        <p>
          Interactive Hangman game using word‑frequency analysis from Kaggle datasets
          to balance difficulty and player experience.
        </p>
      </div>

    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>Contact</h2>
    <div class="card">
      <p>
        I’m open to internship and entry‑level roles in full stack development,
        data, or AI‑related work. Feel free to reach out.
      </p>
      <p>
        <strong>Email:</strong>
        <a href="mailto:praneethaempowers@gmail.com">praneethaempowers@gmail.com</a><br/>
        <strong>LinkedIn:</strong>
        <a href="https://www.linkedin.com/in/praneetha-sripada/" target="_blank">
          linkedin.com/in/praneetha-sripada
        </a><br/>
        <strong>GitHub:</strong>
        <a href="https://github.com/Praneetha-coder" target="_blank">
          github.com/YOUR_GITHUB_USERNAME
        </a>
      </p>
    </div>
  </section>
</main>
</body>
</html>
