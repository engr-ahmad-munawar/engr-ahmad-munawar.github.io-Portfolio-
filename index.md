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
<div class="projects-grid">
  <div class="project-card">
    <h3>Portfolio Website</h3>
    <p>Built with Jekyll & GitHub Pages</p>
    <a href="#">View Project →</a>
  </div>
  <div class="project-card">
    <h3>Mini Game App</h3>
    <p>JS + HTML5 Canvas</p>
    <a href="#">View Project →</a>
  </div>
  <div class="project-card">
    <h3>Blog CMS</h3>
    <p>Markdown-powered blog</p>
    <a href="#">View Project →</a>
  </div>
</div>

<!-- Quick Links -->
<h2>Quick Links 🔗</h2>
<ul>
  <li><a href="/about">About Me</a></li>
  <li><a href="/journey">My Journey</a></li>
  <li><a href="/posts">Posts</a></li>
</ul>

<!-- Social Icons -->
<h2>Connect With Me</h2>
<div class="social">
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
