---
layout: home
title: Aidan 的博客
---

<div class="site-header">
  <h1 class="site-title">{{ site.title }}</h1>
  <p class="site-description">{{ site.description }}</p>
  
  <div class="mt-4">
    <a href="/about" class="btn-primary">了解更多</a>
    <a href="https://github.com/{{ site.github_username }}" class="btn-outline" target="_blank">
      <i class="fab fa-github"></i> GitHub ↗
    </a>
  </div>
  
  <div class="arrow-down">
    <i class="fas fa-chevron-down text-white-50" style="font-size: 2rem;"></i>
  </div>
</div>

<div class="container">
  <div class="section-title">
    <h2>最新文章</h2>
    <p>分享学习笔记与实验心得</p>
  </div>

  <div class="row">
    {% for post in site.posts %}
    <div class="col-md-12">
      <article class="post-card">
        <span class="post-category">{{ post.categories | first }}</span>
        <h3 class="post-title"><a href="{{ post.url }}" style="color: inherit; text-decoration: none;">{{ post.title }}</a></h3>
        <div class="post-meta">
          <i class="far fa-calendar"></i> {{ post.date | date: "%Y年%m月%d日" }}
        </div>
        <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
        <a href="{{ post.url }}" class="read-more">阅读全文 →</a>
      </article>
    </div>
    {% endfor %}
  </div>
</div>

<footer>
  <p>&copy; {{ site.time | date: '%Y' }} {{ site.author }}. 做一个持续成长的计算机专业学生。</p>
  <div class="social-icons">
    <a href="https://github.com/{{ site.github_username }}" target="_blank"><i class="fab fa-github"></i></a>
    <a href="https://twitter.com/{{ site.twitter_username }}" target="_blank"><i class="fab fa-twitter"></i></a>
  </div>
</footer>
