---
layout: page
title: "Hi, I'm Vivek Bhanot"
subtitle: Data Governance, Data Management, BI & Analytics Professional
css: "/css/index.css"
meta-title: "Vivek Bhanot -  Data Governance, Data Management, BI & Analytics Professional"
meta-description: "Data Governance, Data Management, BI & Analytics Professional."
bigimg:
  - "/img/big-imgs/img1.jpg" : "BankTech Asia Conference, Jakarta, Indonesia (2016)"
  - "/img/big-imgs/img2.jpg" : "BankTech Asia Conference, Jakarta, Indonesia (2016)"
  - "/img/big-imgs/img3.jpg" : "BankTech Asia Conference, Jakarta, Indonesia (2016)"
  - "/img/big-imgs/img4.jpg" : "BankTech Asia Conference, Jakarta, Indonesia (2016)"
  - "/img/big-imgs/img6.jpg" : "The Asian Banker Summit - Hanoi, Vietnam (2016)"
  - "/img/big-imgs/img5.jpg" : "Fleming Gulf Back Office Conference - KL, Malaysia (2015)" 
---

<div class="list-filters">
  <a href="/" class="list-filter">All posts</a>
  <span class="list-filter filter-selected">Most Popular</span>
  <a href="/tutorials" class="list-filter">Tutorials</a>
</div>

<div class="posts-list">
  {% for post in site.tags.popular %}
  <article>
    <a class="post-preview" href="{{ post.url | prepend: site.baseurl }}">
	    <h2 class="post-title">{{ post.title }}</h2>
	
	    {% if post.subtitle %}
	    <h3 class="post-subtitle">
	      {{ post.subtitle }}
	    </h3>
	    {% endif %}
      <p class="post-meta">
        Posted on {{ post.date | date: "%B %-d, %Y" }}
      </p>

      <div class="post-entry">
        {{ post.content | truncatewords: 50 | strip_html | xml_escape}}
        <span href="{{ post.url | prepend: site.baseurl }}" class="post-read-more">[Read&nbsp;More]</span>
      </div>
    </a>  
   </article>
  {% endfor %}
</div>
