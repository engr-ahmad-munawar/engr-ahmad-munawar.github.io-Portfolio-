---
layout: home
title: Home
---

<!-- Hero Section -->
<div class="hero" style="background: linear-gradient(135deg, #6a11cb, #2575fc); color: #fff; padding: 6rem 2rem; border-radius: 15px; text-align:center;">
  <h1 id="hero-name" style="font-size: 3rem; margin-bottom: 1rem;">Ahmed Munawar 🚀</h1>
  <p style="font-size: 1.25rem; margin-bottom: 2rem;">Turning ideas into code. Web dev | Projects | Blog</p>
  <div style="font-size: 1.1rem; font-style: italic;" id="typing"></div>
</div>

<!-- Featured Projects -->
<h2 style="margin-top:3rem;">Featured Projects 💎</h2>
<div class="projects-grid" style="display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr)); gap:1.5rem; margin:2rem 0;">
  <div class="project-card" style="padding:1.5rem; border-radius:15px; box-shadow:0 5px 20px rgba(0,0,0,0.1); transition:0.3s;">
    <h3>Portfolio Website</h3>
    <p>Built with Jekyll & GitHub Pages</p>
    <a href="#">View Project →</a>
  </div>
  <div class="project-card" style="padding:1.5rem; border-radius:15px; box-shadow:0 5px 20px rgba(0,0,0,0.1); transition:0.3s;">
    <h3>Mini Game App</h3>
    <p>JS + HTML5 Canvas</p>
    <a href="#">View Project →</a>
  </div>
  <div class="project-card" style="padding:1.5rem; border-radius:15px; box-shadow:0 5px 20px rgba(0,0,0,0.1); transition:0.3s;">
    <h3>Blog CMS</h3>
    <p>Markdown-powered blog</p>
    <a href="#">View Project →</a>
  </div>
</div>

<!-- Quick Links -->
<h2>Quick Links 🔗</h2>
<ul style="margin-bottom:2rem;">
  <li><a href="/about">About Me</a></li>
  <li><a href="/journey">My Journey</a></li>
  <li><a href="/posts">Posts</a></li>
</ul>

<!-- Social Icons -->
<h2>Connect With Me</h2>
<div class="social" style="margin-bottom:2rem;">
  <a href="https://github.com/engr-ahmad-munawar" target="_blank">GitHub</a> |
  <a href="https://www.linkedin.com/in/engr-ahmad-munawar" target="_blank">LinkedIn</a> |
  <a href="mailto:hello@ahmedmunawar.com">Email</a>
</div>

<!-- Dark Mode Toggle -->
<button onclick="document.body.classList.toggle('dark')">Toggle Dark Mode</button>

<!-- Typing Animation Script -->
<script>
  const texts = ["Web Developer 💻", "Tech Enthusiast 🚀", "Creative Coder 🎨"];
  let count = 0, index = 0, currentText = "", letter = "";
  (function type(){
    if(count === texts.length) count = 0;
    currentText = texts[count];
    letter = currentText.slice(0, ++index);
    document.getElementById("typing").textContent = letter;
    if(letter.length === currentText.length){ count++; index=0; setTimeout(type,1000); }
    else{ setTimeout(type,150); }
  }());
</script>
