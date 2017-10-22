---
layout: default
title: Nouvelles
image: assets/images/products.jpg
color: orange
order: 2
---
<div class="columns">
  <div class="column">
    <div class="is-flex tile is-parent is-child">
      <div class="fb-page" data-href="https://www.facebook.com/mielsbersyla" data-tabs="timeline, events" data-small-header="true"
        data-adapt-container-width="true" data-hide-cover="true" data-show-facepile="true" data-width="500">
      </div>
    </div>
  </div>
  <div class="column">
    {% for post in site.posts %}
      <div class="tile is-parent is-child">
        <div class="card">
          <header class="card-header">
            <p class="card-header-title">
              {{ post.title }}
            </p>
          </header>
          <div class="card-content">
            <div class="content">
              {{ post.excerpt }}
            </div>
          </div>
          <footer class="card-footer">
            <a href="{{ post.url }}" class="card-footer-item">
              Lire la suite
            </a>
          </footer>
        </div>
      </div>
    {% endfor %}
  </div>
</div>