<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Michael Takil – Professional Portfolio</title>
<style>
  body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background: black;
    color: gold;
    overflow-x: hidden;
  }

  /* Glowing star particles */
  .star {
    position: absolute;
    width: 2px;
    height: 2px;
    background: gold;
    border-radius: 50%;
    animation: twinkle 2s infinite ease-in-out alternate;
  }

  @keyframes twinkle {
    0% { opacity: 0.2; transform: scale(0.5); }
    50% { opacity: 1; transform: scale(1.2); }
    100% { opacity: 0.2; transform: scale(0.5); }
  }

  header {
    text-align: center;
    margin-top: 40px;
    margin-bottom: 50px;
  }

  h1 { font-size: 3rem; margin-bottom: 0.5rem; }
  h2 { font-size: 1.5rem; margin-bottom: 2rem; font-weight: normal; }

  section {
    padding: 0 40px 60px 40px;
  }

  h3.section-title {
    text-align: center;
    margin-bottom: 30px;
    font-size: 2rem;
    text-decoration: underline;
    text-decoration-color: gold;
    text-underline-offset: 8px;
  }

  .projects {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 20px;
  }

  .card {
    background: rgba(0,0,0,0.8);
    border: 2px solid gold;
    border-radius: 12px;
    padding: 20px;
    text-align: center;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .card:hover {
    transform: translateY(-10px);
    box-shadow: 0 0 20px gold;
  }

  a {
    color: gold;
    text-decoration: none;
    font-weight: bold;
  }

  a:hover {
    text-decoration: underline;
  }
</style>
</head>
<body>

<!-- Glowing stars animation -->
<script>
  const numStars = 150;
  for(let i=0;i<numStars;i++){
    const star = document.createElement('div');
    star.className = 'star';
    star.style.top = Math.random() * window.innerHeight + 'px';
    star.style.left = Math.random() * window.innerWidth + 'px';
    star.style.animationDuration = (Math.random()*3 + 1) + 's';
    document.body.appendChild(star);
  }
</script>

<header>
  <h1>Michael Takil</h1>
  <h2>Full-Stack & AI Engineer | ICT Entrepreneur | Ethical Hacking Trainee</h2>
</header>

<!-- Web & Cloud Applications -->
<section>
  <h3 class="section-title">Web & Cloud Applications</h3>
  <div class="projects">
    <div class="card">
      <h4>StepUp Loan</h4>
      <p>Loan management system with tier-based borrowing, repayment tracking, and real-time dashboards.</p>
      <p><strong>Tech:</strong> HTML, CSS, JS, Firebase, Cloud Hosting</p>
      <a href="https://stepup-loan.web.app" target="_blank">Live Demo</a>
    </div>
    <div class="card">
      <h4>National Transport System</h4>
      <p>RTA checkpoint monitoring & vehicle/license management with live alerts and reporting dashboards.</p>
      <p><strong>Tech:</strong> HTML, CSS, JS, Firebase, PostgreSQL</p>
      <a href="https://national-transport-system.web.app" target="_blank">Live Demo</a>
    </div>
    <div class="card">
      <h4>Road Traffic Authority</h4>
      <p>Cloud-based system for vehicle registration, driver licensing, and traffic enforcement.</p>
      <p><strong>Tech:</strong> Node.js, MongoDB, REST APIs, Cloud Hosting</p>
      <a href="https://road-traffic-authority.web.app" target="_blank">Live Demo</a>
    </div>
    <div class="card">
      <h4>Live Health Tracking & Monitoring System</h4>
      <p>Centralized platform for hospital/clinic operations, patient records, and real-time reporting.</p>
      <p><strong>Tech:</strong> Firebase, PostgreSQL, Cloud Hosting</p>
      <p>Internal</p>
    </div>
  </div>
</section>

<!-- AI & Multimedia Platforms -->
<section>
  <h3 class="section-title">AI & Multimedia Platforms</h3>
  <div class="projects">
    <div class="card">
      <h4>KinaChat</h4>
      <p>AI-powered multimedia chat platform. Users generate images, videos, music, voice outputs, translations, and Unity projects.</p>
      <p><strong>Tech:</strong> NLP, React, Firebase, GCP</p>
      <p>Internal</p>
    </div>
    <div class="card">
      <h4>NudePixel</h4>
      <p>AI platform for text-to-image, text-to-video, image-to-video generation. Optimized inference on GCP GPU.</p>
      <p><strong>Tech:</strong> Node.js, React, GCP, AI</p>
      <p>Internal</p>
    </div>
    <div class="card">
      <h4>RewardRush</h4>
      <p>Fast-paced mobile game with real-time leaderboard integration.</p>
      <p><strong>Tech:</strong> Java, Firebase</p>
      <a href="https://play.google.com/store/apps/details?id=com.TakilGame.RewardRush" target="_blank">Google Play</a>
    </div>
  </div>
</section>

<!-- Government & Analytics Systems -->
<section>
  <h3 class="section-title">Government & Analytics Systems</h3>
  <div class="projects">
    <div class="card">
      <h4>MorobeLiquor Track</h4>
      <p>Digitized liquor licensing & compliance monitoring system for Morobe Provincial Government.</p>
      <p><strong>Tech:</strong> HTML, CSS, JS, Firebase, Leaflet.js</p>
      <a href="https://morobeliquor-track.web.app/" target="_blank">Live Demo</a>
    </div>
    <div class="card">
      <h4>RPNGC Live Monitoring & Tracking System</h4>
      <p>Police operations platform with case management, incident mapping, dashboards, and notifications.</p>
      <p><strong>Tech:</strong> HTML, CSS, JS, Firebase</p>
      <p>Internal</p>
    </div>
    <div class="card">
      <h4>Connect PNG – DoWH Dashboard</h4>
      <p>National infrastructure monitoring dashboard with KPIs, maps, and real-time reporting.</p>
      <p><strong>Tech:</strong> HTML, CSS, JS, Chart.js, Leaflet.js, Firebase</p>
      <p>Internal</p>
    </div>
    <div class="card">
      <h4>ICCC Live Price Tracking System</h4>
      <p>Nationwide price monitoring system with dashboards, GPS mapping, automated violation detection, and audit-ready reporting.</p>
      <p><strong>Tech:</strong> HTML, CSS, JS, Firebase</p>
      <p>Internal</p>
    </div>
  </div>
</section>

</body>
</html>
