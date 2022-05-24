---
layout: home
---



{% assign home = site.home | sort: 'date' | reverse %}
{% for home in home %}


 <ul class="cols cover {{post.color}}">
  {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
 <li>
 <a href="{{ home.url }}" rel="bookmark" title="Permalink to The Revenge of the Hot Water Bottle">
                        <h2 class="entry-title"> {{ home.title }}</h2>
                    </a>
                    <a class="category" href="https://web.archive.org/web/20220305191730/https://solar.lowtechmagazine.com/obsolete-technology.html">Obsolete Technology</a>
                    <p class="index-summary">{{ home.teaser }}</p>
                    <time class="published" datetime="2022-01-20T00:00:00+01:00">{{ home.date | date_to_string }}</time>
                </li>
                <li>
                    <a href="https://web.archive.org/web/20220305191730/https://solar.lowtechmagazine.com/2022/01/the-revenge-of-the-hot-water-bottle.html" rel="bookmark" title="Permalink to The Revenge of the Hot Water Bottle">
                        <div class="featured-img" style="background-image: url('{{ home.featured }}');"></div>
                    </a>
                </li>
{% endfor %}
            </ul>
