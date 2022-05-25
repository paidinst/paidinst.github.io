---
layout: home
---


 <ul class="cols recent">
  {% assign lectures = site.lectures | sort: 'date' | reverse %}
  {% for lectures in lectures %}
                    
                <li class="{{ lectures.color }}">
                    <article>
                        <a href="{{ lectures.url }}" rel="bookmark" title="Permalink to The Printed Website: Volume III &amp; The Comments">
                            <div class="featured-img" style="border: 1px solid #348da8;background-image: url('{{ lectures.featured }}');"></div>
                            <h2 class="entry-title">
                            {{ lectures.title }}
                            
                            </h2>
                        </a>
                        <a class="category" href="https://web.archive.org/web/20220305191730/https://solar.lowtechmagazine.com/low-tech-solutions.html">Low-tech solutions</a>
                        <p class="index-summary">{{ lectures.teaser }}</p>
                       <!-- <time class="published" datetime="2021-12-02T00:00:00+01:00">{{ lectures.date | date_to_string }}</time>-->
                    </article>
                </li>
        {% endfor %}       
            </ul>


