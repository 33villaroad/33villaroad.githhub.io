---
layout: page
title: Gallery
permalink: /gallery/
---

<div class="pswp-gallery" id="property-gallery">
	<!-- Replace these placeholders with your own images -->
	<a href="/assets/images/living-room.jpg" data-pswp-width="1200" data-pswp-height="800" data-pswp-title="Living Room">
		<img src="/assets/images/living-room.jpg" alt="Living Room" style="width:300px; margin:10px;" />
	</a>
	<a href="/assets/images/kitchen.jpg" data-pswp-width="1200" data-pswp-height="800" data-pswp-title="Kitchen">
		<img src="/assets/images/kitchen.jpg" alt="Kitchen" style="width:300px; margin:10px;" />
	</a>
	<a href="/assets/images/interior-upstairs.jpg" data-pswp-width="1200" data-pswp-height="800" data-pswp-title="Bedroom">
		<img src="/assets/images/interior-upstairs.jpg" alt="Bedroom" style="width:300px; margin:10px;" />
	</a>
</div>

<link rel="stylesheet" href="/assets/js/photoswipe/photoswipe.css">
<script type="module">
import PhotoSwipeLightbox from '/assets/js/photoswipe/photoswipe-lightbox.esm.js';
const lightbox = new PhotoSwipeLightbox({
  gallery: '#property-gallery',
  children: 'a',
  pswpModule: () => import('/assets/js/photoswipe/photoswipe.esm.js')
});
lightbox.init();
</script>
