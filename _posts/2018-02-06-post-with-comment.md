---
title: "Post: With comment"
excerpt: "This is to test the comment section"
tags:
  - Jun
  - Site tests
---
{% capture fig_img %}
![Foo]({{ "/assets/images/coding-image.jpg" | absolute_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Some random image</figcaption>
</figure>
