---
title: Gallery
permalink: /gallery/
layout: default
photos:
- src: /images/IMG_3347.jpeg
  alt: Photo of Liam outside of store (kenya)
  span: 1
- src: /images/IMG_1958.jpg
  alt: Photo of The Chonks at the factory
  span: 1
- src: /images/IMG_1999.jpeg
  alt: The Chonks at the crest
  span: 2
- src: /images/IMG-3175.JPG
  alt: TruckBox
  span: 1
- src: /images/IMG-1411.JPG
  alt: placeholder 
  span: 1
- src: /images/IMG-1339.JPG
  alt: Maasai Village
  span: 2
- src: /images/rsz_img-3083.jpg
  alt: placeholder image
  span: 2
- src: /images/rsz_img-3177.jpg
  alt: Liam Tuning Bass
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