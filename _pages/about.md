---
permalink: /
title: "Hello There,:wave: I'm Nixon"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I specialize in building and deploying real-time computer vision platforms, generative AI models, and transformer-based systems across diverse industries. With a deep passion for data-driven solutions, I have worked extensively to create scalable, intelligent systems. My expertise spans machine learning, deep learning, and generative AI, focusing on natural language processing, computer vision, and decision-making automation.

I share insights from my work on these innovations, offering a behind-the-scenes look at how AI is transforming industries and creating new possibilities. Join me as I delve into the latest trends, tools, and practical applications in the rapidly evolving world of data science and Generative AI.

### Articles

[Custom DataLoader for Machine Learning in Python: A Comprehensive Guide](https://nixongenoa.github.io/posts/2024/10/Custom-DataLoader-for-Machine-Learning-in-Python-A-Comprehensive-Guide/)
In this blog, we'll cover how to create a custom DataLoader in Python, explore batching, shuffling, custom transformations, and load multidimensional data.

{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    <h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}

