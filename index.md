---
layout: home
title: Welcome to My Personal Site
---

<div class="home-section">
  <img src="https://neeko-copilot.bytedance.net/api/text_to_image?prompt=professional%20portrait%20photo%20of%20a%20young%20asian%20developer%20with%20glasses%20smiling%20in%20modern%20office%2C%20clean%20background%2C%20professional%20lighting&image_size=square" alt="Aidan" class="avatar">
  
  <h1>Hi, I'm Aidan</h1>
  
  <p class="lead" style="font-size: 1.3rem; color: #666; margin: 1.5rem 0;">
    A passionate Full-Stack Developer and Tech Enthusiast
  </p>
  
  <p style="max-width: 600px; margin: 0 auto 2rem;">
    I love building innovative web applications and exploring new technologies. 
    Currently focused on creating beautiful, functional, and scalable solutions.
  </p>
  
  <a href="/about" class="btn btn-primary">Learn More About Me</a>
</div>

<hr style="margin: 3rem 0;">

## Featured Projects

<div class="row">
  <div class="col-md-4">
    <div class="card">
      <div class="card-body">
        <h3 class="card-title">Project One</h3>
        <p class="card-text">A modern web application with React and Node.js backend.</p>
        <a href="#" class="btn btn-outline-primary btn-sm">View Project</a>
      </div>
    </div>
  </div>
  
  <div class="col-md-4">
    <div class="card">
      <div class="card-body">
        <h3 class="card-title">Project Two</h3>
        <p class="card-text">Data visualization dashboard with D3.js and Python.</p>
        <a href="#" class="btn btn-outline-primary btn-sm">View Project</a>
      </div>
    </div>
  </div>
  
  <div class="col-md-4">
    <div class="card">
      <div class="card-body">
        <h3 class="card-title">Project Three</h3>
        <p class="card-text">Mobile-first e-commerce platform with Vue.js.</p>
        <a href="#" class="btn btn-outline-primary btn-sm">View Project</a>
      </div>
    </div>
  </div>
</div>

<hr style="margin: 3rem 0;">

## Latest Posts

<div class="row">
  {% for post in site.posts limit:3 %}
  <div class="col-md-4 post-card">
    <div class="card">
      <div class="card-body">
        <h4 class="card-title">{{ post.title }}</h4>
        <p class="text-muted" style="font-size: 0.9rem;">{{ post.date | date: "%B %d, %Y" }}</p>
        <p class="card-text">{{ post.excerpt | truncatewords: 20 }}</p>
        <a href="{{ post.url }}" class="btn btn-link">Read More</a>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
