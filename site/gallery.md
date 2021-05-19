---
title: Gallery
permalink: /gallery/
layout: default
photos:
- src: https://via.placeholder.com/200
  alt: placeholder image
  span: 1
- src: https://via.placeholder.com/200
  alt: placeholder image
  span: 1
- src: https://via.placeholder.com/400x200
  alt: placeholder image
  span: 2
- src: https://via.placeholder.com/200
  alt: placeholder image
  span: 1
- src: https://via.placeholder.com/200
  alt: placeholder image
  span: 1
- src: https://via.placeholder.com/400x200
  alt: placeholder image
  span: 2
- src: https://via.placeholder.com/200
  alt: placeholder image
  span: 2
- src: https://via.placeholder.com/200
  alt: placeholder image
  span: 1
- src: https://via.placeholder.com/400x200
  alt: placeholder image
  span: 1
---

<section class="gallery" data-masonry='{ "itemSelector": ".grid-item", "columnWidth": ".grid-sizer", "gutter": ".gutter-sizer", "resize": true }'>
<div class="grid-sizer"></div>
<div class="gutter-sizer"></div>
{% for photo in page.photos %}
  <div class="grid-item {% if photo.span == 2 %}grid-item-2{% endif %}">
    <img src="{{photo.src}}" alt="{{photo.alt}}">
  </div>
{% endfor %}
</section>