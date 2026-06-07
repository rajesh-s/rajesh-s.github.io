---
layout: post
date: 2026-04-22 15:59:00-0400
title:   I was nominated to attend the 2026 IEEE Laureate Forum and Honors Ceremony in NYC.
inline: false
related_posts: false
---

Recently, I had the opportunity to attend two signature IEEE events in New York that celebrate innovation in engineering and technology: the 2026 IEEE Laureate Forum and the IEEE Honors Ceremony.

The Laureate Forum was dedicated to recognizing outstanding young professionals and early career researchers from around the world. It was a meaningful opportunity to learn from global technology leaders, connect with the broader IEEE community, and reflect on the many ways engineering continues to shape our world, especially in these times of rapid change.  My sincere thanks to Eric Van Hensbergen for the nomination, and to IEEE-USA Awards & Recognition for making this opportunity possible. The forum offered the opportunity to hear from distinguished award recipients whose work spans a wide range of disciplines, including pioneers behind inventing technologies such as the 3D FinFET and the GPU. A theme that resonated with me was that the impact of engineering is not measured by technical progress alone, but also by the ways technology improves lives and serves society. This came through in many forms, from Giorgia Lupi’s work in storytelling to the inspiring contributions of Marian Croak in wireless communication and Mariana Costa Checa in expanding societal reach.

The experience concluded with the IEEE Honors Ceremony, where I had the privilege of presenting the Arm sponsored James Clerk Maxwell Medal alongside my colleague Hrutvik Kanabar. It was humbling to see IEEE’s highest level awards recognize global leaders and innovators whose work has had such a lasting impact on engineering and technology.

As a Computer Architect, a personal highlight was meeting two people whose work I have long admired: NVIDIA co-founders Jensen Huang and Chris Malachowsky, this year’s recipients of the prestigious IEEE Medal of Honor and Robert N. Noyce Medal, respectively. Somewhere along the speech, Jensen said, “In all that I’ve learned, the purpose is not in advancing technology alone, or just in building successful companies. The purpose is ultimately your family and the people that you love, and it is for them that we do this when we pursue the things that we do.” And that stuck with me.

<style>
.square {
  aspect-ratio: 1 / 1;
  width: 100%;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
}

.square img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>

<div class="row mt-3">
  {% for i in (1..3) %}
    {% assign img_path = "assets/img/ieee" | append: i | append: ".jpg" %}

    <div class="col-sm-4 mt-3 mt-md-0">
      <div class="square">
        {% include figure.liquid
          loading="eager"
          path=img_path
          class="img-fluid rounded z-depth-1"
        %}
      </div>
    </div>
  {% endfor %}
</div>