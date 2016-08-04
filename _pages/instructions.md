---
layout: page
title: Instructions
permalink: /instructions/
---

<aside>
Reminder: visual instructions are not included. It is the sighted parent/teacher/friend's responsibility to have access to the instructions to check the blind builder, and to have a physical copy of the set. Graphical instructions can be downloaded from Lego's website. I do not sell sets, I simply provide an alternative instruction format.
</aside>
<ul class="post-list">
    <h2>0-50 pieces</h2>
      {% for instruction in site.instructions %}
        {% if instruction.pieces <= 50 %}
        <li> 
          <img class="instructions-img" src="" alt="instruction.alt" width="80" height="80">
          <div class="instructions-body">
          <h2>
            <a class="post-link" href="{{ instruction.url | prepend: site.baseurl }}">{{ instruction.title }}</a>
          </h2>
          <a href="{{ instruction.url | prepend: site.baseurl }}">Download</a>
          <a href="{{instruction.link}}">More Information</a>
      	</div>
        </li>
        {% endif %}
    {% endfor %}
    <h2>50-100 pieces</h2>
      {% for instruction in site.instructions %}
        {% if instruction.pieces > 50 and instruction.pieces <= 100   %}
        <li> 
          <img class="instructions-img" src="" alt="instruction.alt" width="80" height="80">
          <div class="instructions-body">
          <h2>
            <a class="post-link" href="{{ instruction.url | prepend: site.baseurl }}">{{ instruction.title }}</a>
          </h2>
          <a href="{{ instruction.url | prepend: site.baseurl }}">Download</a>
          <a href="{{instruction.link}}">More Information</a>
        </div>
        </li>
        {% endif %}
    {% endfor %}
    <h2>100-500 pieces</h2>
      {% for instruction in site.instructions %}
        {% if instruction.pieces > 100 and instruction.pieces <= 500   %}
        <li> 
          <img class="instructions-img" src="" alt="instruction.alt" width="80" height="80">
          <div class="instructions-body">
          <h2>
            <a class="post-link" href="{{ instruction.url | prepend: site.baseurl }}">{{ instruction.title }}</a>
          </h2>
          <a href="{{ instruction.url | prepend: site.baseurl }}">Download</a>
          <a href="{{instruction.link}}">More Information</a>
        </div>
        </li>
        {% endif %}
    {% endfor %}
    <h2>500-1000 pieces</h2>
      {% for instruction in site.instructions %}
        {% if instruction.pieces > 500 and instruction.pieces <= 1000   %}
        <li> 
          <img class="instructions-img" src="" alt="instruction.alt" width="80" height="80">
          <div class="instructions-body">
          <h2>
            <a class="post-link" href="{{ instruction.url | prepend: site.baseurl }}">{{ instruction.title }}</a>
          </h2>
          <a href="{{ instruction.url | prepend: site.baseurl }}">Download</a>
          <a href="{{instruction.link}}">More Information</a>
        </div>
        </li>
        {% endif %}
    {% endfor %}
    <h2>1000-2000 pieces</h2>
      {% for instruction in site.instructions %}
        {% if instruction.pieces > 1000 and instruction.pieces <= 2000   %}
        <li> 
          <img class="instructions-img" src="" alt="instruction.alt" width="80" height="80">
          <div class="instructions-body">
          <h2>
            <a class="post-link" href="{{ instruction.url | prepend: site.baseurl }}">{{ instruction.title }}</a>
          </h2>
          <a href="{{ instruction.url | prepend: site.baseurl }}">Download</a>
          <a href="{{instruction.link}}">More Information</a>
        </div>
        </li>
        {% endif %}
    {% endfor %}
    <h2>2000+ pieces</h2>
      {% for instruction in site.instructions %}
        {% if instruction.pieces > 2000   %}
        <li> 
          <img class="instructions-img" src="" alt="instruction.alt" width="80" height="80">
          <div class="instructions-body">
          <h2>
            <a class="post-link" href="{{ instruction.url | prepend: site.baseurl }}">{{ instruction.title }}</a>
          </h2>
          <a href="{{ instruction.url | prepend: site.baseurl }}">Download</a>
          <a href="{{instruction.link}}">More Information</a>
        </div>
        </li>
        {% endif %}
    {% endfor %}

</ul>