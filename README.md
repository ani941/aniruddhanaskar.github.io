# aniruddhanaskar.github.io
Hi, I'm ani
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Aniruddha Naskar Portfolio</title>
  <link rel="stylesheet" href="style.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700;900&display=swap" rel="stylesheet">
</head>
<body>
  <section class="intro">
    <div class="intro-content">
      <div class="intro-text">
        <h1 class="glow-title">Aniruddha Naskar</h1>
        <p class="tagline">I build intelligent systems that blend AI and automation with real-world purpose.</p>
        <p class="summary">
          Passionate about AI, automation, and futuristic technologies. Experienced in building smart systems, 
          IoT projects, and interactive AI assistants like Jarvis X.
        </p>

        <div class="skills">
          <span class="skill">AI</span>
          <span class="skill">Python</span>
          <span class="skill">IoT</span>
          <span class="skill">Automation</span>
          <span class="skill">Web Dev</span>
        </div>

        <div class="intro-buttons">
          <a href="#projects" class="btn">Projects</a>
          <a href="#contact" class="btn secondary">Contact</a>
          <a href="/resume.pdf" class="btn download">Download Resume</a>
        </div>

        <div class="social-icons">
          <a href="https://github.com/aniruddha" target="_blank">GitHub</a>
          <a href="https://linkedin.com/in/aniruddha" target="_blank">LinkedIn</a>
          <a href="https://twitter.com/aniruddha" target="_blank">Twitter</a>
        </div>
      </div>

      <div class="intro-image">
        <img src="assets/images/profile.png" alt="Aniruddha Naskar">
      </div>
    </div>

    <div class="floating-circles">
      <span></span>
      <span></span>
      <span></span>
      <span></span>
      <span></span>
    </div>
  </section>
</body>
</html>
/* Google Fonts */
body {
  font-family: 'Roboto', sans-serif;
  margin: 0;
  padding: 0;
  background: linear-gradient(135deg, #1f1c2c, #928dab);
  color: #fff;
  overflow-x: hidden;
}

.intro {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  padding: 0 2rem;
}

.intro-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  width: 100%;
  z-index: 2;
}

.intro-text {
  max-width: 600px;
}

.glow-title {
  font-size: 3rem;
  font-weight: 900;
  text-shadow: 0 0 10px #ff00ff, 0 0 20px #ff00ff, 0 0 30px #ff00ff;
}

.tagline {
  font-size: 1.2rem;
  margin: 10px 0 20px;
}

.summary {
  font-size: 1rem;
  line-height: 1.5;
  margin-bottom: 20px;
}

.skills {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-bottom: 20px;
}

.skill {
  background: rgba(255, 255, 255, 0.1);
  padding: 5px 12px;
  border-radius: 20px;
  font-size: 0.9rem;
  transition: 0.3s;
}
.skill:hover {
  background: #ff00ff;
  cursor: pointer;
}

.intro-buttons .btn {
  padding: 10px 20px;
  margin-right: 10px;
  border-radius: 30px;
  text-decoration: none;
  color: #fff;
  background: linear-gradient(90deg, #ff00ff, #ff69b4);
  transition: 0.3s;
}
.intro-buttons .btn:hover {
  transform: translateY(-5px);
  box-shadow: 0 5px 20px rgba(255, 0, 255, 0.5);
}

.intro-buttons .secondary {
  background: transparent;
  border: 2px solid #fff;
}

.intro-buttons .download {
  background: #00ffff;
  color: #000;
}

.social-icons a {
  margin-right: 15px;
  color: #fff;
  text-decoration: none;
  font-weight: 600;
}
.social-icons a:hover {
  color: #ff00ff;
}

.intro-image img {
  max-width: 300px;
  border-radius: 50%;
  border: 4px solid #ff00ff;
  box-shadow: 0 0 30px #ff00ff;
}

.floating-circles span {
  position: absolute;
  display: block;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.1);
  animation: float 10s infinite;
}
.floating-circles span:nth-child(1) { width: 80px; height: 80px; top: 10%; left: 20%; }
.floating-circles span:nth-child(2) { width: 50px; height: 50px; top: 30%; left: 70%; }
.floating-circles span:nth-child(3) { width: 100px; height: 100px; top: 60%; left: 40%; }
.floating-circles span:nth-child(4) { width: 60px; height: 60px; top: 80%; left: 80%; }
.floating-circles span:nth-child(5) { width: 30px; height: 30px; top: 50%; left: 10%; }

@keyframes float {
  0% { transform: translateY(0) rotate(0deg); }
  50% { transform: translateY(-20px) rotate(180deg); }
  100% { transform: translateY(0) rotate(360deg); }
}

@media (max-width: 900px) {
  .intro-content {
    flex-direction: column;
    text-align: center;
  }
  .intro-image {
    margin-top: 20px;
  }
}
