---
layout: page
title: projects
permalink: /projects/
description: 
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  <!-- Manually add projects without relying on _projects folder -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-2">
      <!-- Project 1 -->
      <div class="col">
        <div class="card">
          <img src="/assets/images/ml_project.jpg" class="card-img-top" alt="Machine Learning Project">
          <div class="card-body">
            <h5 class="card-title">Machine Learning Project</h5>
            <p class="card-text">A machine learning project to predict stock prices.</p>
            <a href="https://github.com/user/ml-project" class="btn btn-primary">Learn more</a>
          </div>
        </div>
      </div>
      <!-- Project 2 -->
      <div class="col">
        <div class="card">
          <img src="/assets/images/website.jpg" class="card-img-top" alt="Personal Website">
          <div class="card-body">
            <h5 class="card-title">Personal Website</h5>
            <p class="card-text">A personal website built with Jekyll.</p>
            <a href="https://user.github.io/" class="btn btn-primary">Learn more</a>
          </div>
        </div>
      </div>
    </div>
  </div>
  {% else %}
  <div class="grid">
    <!-- Project 1 -->
    <div class="project-card">
      <img src="/assets/images/ml_project.jpg" alt="Machine Learning Project">
      <h3>Machine Learning Project</h3>
      <p>A machine learning project to predict stock prices.</p>
      <a href="https://github.com/user/ml-project">Learn more</a>
    </div>
    <!-- Project 2 -->
    <div class="project-card">
      <img src="/assets/images/website.jpg" alt="Personal Website">
      <h3>Personal Website</h3>
      <p>A personal website built with Jekyll.</p>
      <a href="https://user.github.io/">Learn more</a>
    </div>
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

  <!-- Manually add projects without relying on _projects folder -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-2">
      <!-- Project 1 -->
      <div class="col">
        <div class="card">
          <img src="/assets/images/ml_project.jpg" class="card-img-top" alt="Machine Learning Project">
          <div class="card-body">
            <h5 class="card-title">Machine Learning Project</h5>
            <p class="card-text">A machine learning project to predict stock prices.</p>
            <a href="https://github.com/user/ml-project" class="btn btn-primary">Learn more</a>
          </div>
        </div>
      </div>
      <!-- Project 2 -->
      <div class="col">
        <div class="card">
          <img src="/assets/images/website.jpg" class="card-img-top" alt="Personal Website">
          <div class="card-body">
            <h5 class="card-title">Personal Website</h5>
            <p class="card-text">A personal website built with Jekyll.</p>
            <a href="https://user.github.io/" class="btn btn-primary">Learn more</a>
          </div>
        </div>
      </div>
    </div>
  </div>
  {% else %}
  <div class="grid">
    <!-- Project 1 -->
    <div class="project-card">
      <img src="/assets/images/ml_project.jpg" alt="Machine Learning Project">
      <h3>Machine Learning Project</h3>
      <p>A machine learning project to predict stock prices.</p>
      <a href="https://github.com/user/ml-project">Learn more</a>
    </div>
    <!-- Project 2 -->
    <div class="project-card">
      <img src="/assets/images/website.jpg" alt="Personal Website">
      <h3>Personal Website</h3>
      <p>A personal website built with Jekyll.</p>
      <a href="https://user.github.io/">Learn more</a>
    </div>
  </div>
  {% endif %}
{% endif %}
</div>
