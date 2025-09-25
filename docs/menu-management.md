---
title: Menu Management
layout: docs
---


# Menu Management

```` ruby
# Gemfile
gem 'jekyll-archives'
gem "jekyll-sitemap"
gem "jekyll-seo-tag"
````

Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio dignissimos rerum soluta expedita ducimus voluptas suscipit accusantium non reprehenderit saepe? A, provident. Distinctio sint aut similique fuga, recusandae esse aliquid?


````liquid
{% raw %}
  {% assign home_testimonials = site.data.testimonials | where: 'location', 'home' %}
    {% for testimonial in home_testimonials  limit :3 %}  
      <div class="col">
        {% include _testimonial.html testimonial=testimonial %}
      </div>
    {% endfor %}
 {% endraw %}   
````