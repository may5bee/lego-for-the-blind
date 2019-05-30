---
layout: page
title: instructions
permalink: /instructions/
---

<div class="content-section">
<!-- <div class="row">
<div class="col-sm-6">


</div>
</div> -->


    {% for instruction in site.instructions %}
      

    <div class="mini-section">

       <!--  <a href="{{ instruction.url | prepend: site.baseurl }}">
        <img class="instructions-img" src="{{instruction.img}}" alt="instruction.alt" width="80" height="80"></a> -->
        

        <a href="{{ instruction.url | prepend: site.baseurl }}"><h4>
          {{ instruction.title }}
        </h4></a>
        <p>#{{ instruction.setnumber }} | {{ instruction.pieces }} Pieces</p>
        <!-- <a href="{{ instruction.url | prepend: site.baseurl }}">Download</a>
        <a href="{{instruction.link}}">More Information</a> -->
    
    </div>
    {% endfor %}



</div>
