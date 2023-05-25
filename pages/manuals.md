---
layout: page
show_meta: false
title: "EarQuiz Manuals"
permalink: "/manuals/"
---

### <a href="{{ site.url }}{{ site.baseurl }}/manuals/earquiz-frequencies-help/">EarQuiz Frequencies Help</a>
### EarQuiz Frequencies Tutorial Video

<ul>
    {% for post in site.categories.manuals %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>