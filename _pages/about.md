---
layout: page
permalink: /
title: about
nav: About
description: <a href="https://www.deepmind.com/" class="page-description" target="_blank">Google DeepMind</a> • <a href="https://research.google/teams/brain/" class="page-description" target="_blank">Google Research - Brain Team</a>
address: <a href="https://www.google.com/maps/place/Googleplex/@37.4220656,-122.0840897,15z/data=!4m2!3m1!1s0x0:0x6c296c66619367e0?sa=X&ved=2ahUKEwjX-_PLwpv_AhXFlWoFHdJPChsQ_BJ6BAhUEAg" class="page-description" target="_blank">Google DeepMind, Mountain View, CA</a>
---

<div class="col p-0 pt-4 pb-4">
  <h1 class="pb-3 title text-left font-weight-bold">Rishabh Joshi</h1>
  <h6 class="m-0 mb-2" style="font-size: 0.83em;">{{ page.description }}</h6>
  {% if page.address %}
      <h6 class="m-0 mb-2" style="font-size: 0.83em;">{{ page.address }}</h6>
  {% endif %}
</div>

<!-- Introduction -->

<div style="display: flex; flex-wrap: wrap;">
    <div class="text-justify p-0">
        <div class="col-xs-12 col-sm-6 p-0 pt-2 pb-sm-2 pb-4 pl-sm-4 text-center" style="float: right;">
          <img class="profile-img img-responsive" src="{{ 'prof_pic.jpg' | prepend: '/assets/img/' | prepend: site.baseurl | prepend: site.url }}">
        </div>

        <p>
  I am a software engineer working on language research at Google Deepmind (formerly Google Research - Brain Team). My current research focus is on improving the generation and alignment capabilities of large language models. Before joining Google, I did my research masters in Language Technologies (MLT) from <a href="http://www.lti.cs.cmu.edu/" target="_blank">Language Technologies Institute</a>, <a href="http://www.cs.cmu.edu/" target="_blank">School of Computer Science</a> at <a href="http://www.cmu.edu/" target="_blank">Carnegie Mellon University</a>, co-advised by <a href="http://www.cs.cmu.edu/~awb/" target="_blank">Alan W Black</a>, <a href="http://www.cs.cmu.edu/~ytsvetko/" target="_blank">Yulia Tsvetkov</a> and <a href="http://www.cs.cmu.edu/~air/" target="_blank">Alex Rudnicky</a>. I'm also a member of <a href="https://tsvetshop.github.io/" target="_blank">Tsvetshop</a>.
        </p>

        <p>
  My current research focus is on post-training and alignment, including RLHF and preference optimization of Large Language Models as part of the Gemini Team at Google DeepMind. I'm responsible for publishing papers and landing research ideas to improve Google's Gemini model. I'm also interested in self-improving language models. My research in CMU focused dialogue systems, interpretability and text summarization.
        </p>

	<p>
    Before I joined CMU, I worked in Samsung Research Institute, Bangalore, India where I was working in the Voice Intelligence Team on dialogue systems and chat-bots. Before that, I spent a wonderful semester working with <a href="http://talukdar.net" target="_blank">Partha Talukdar</a> at <a href="http://malllabiisc.github.io/" target="_blank">Machine and Language Learning (MALL) Lab</a> in the <a href="https://www.iisc.ac.in/" target="_blank">Indian Institute of Science, Bangalore</a>. I graduated with a B.Eng. in Computer Science from <a href="http://www.bits-pilani.ac.in/pilani/" target="_blank">Birla Institute of Technology and Science, Pilani</a>, India.
    In my Bachelor's thesis, I worked on incorporating external knowledge in distantly supervised neural relation extraction methods as part of iNELL (which is based on <a href='http://rtw.ml.cmu.edu/rtw/' target='_blank'>NELL</a>).
	</p>
    </div>
</div>


<!-- News -->
<div class="news mt-3 p-0">
  <h3 class="title mb-4 p-0">News</h3>
  {% assign news = site.news | reverse %}
  {% for item in news limit: site.news_limit %}
    <div class="row p-0">
      <div class="col-sm-2 p-0">
        <span class="badge danger-color-dark darken-1 font-weight-bold text-uppercase align-middle date ml-3">
          {{ item.date | date: "%b %-d, %Y" }}
        </span>
      </div>
      <div class="col-sm-10 mt-2 mt-sm-0 ml-3 ml-md-0 p-0 font-weight-light text">
        <p>{{ item.content | remove: '<p>' | remove: '</p>' | emojify }}</p>
      </div>
    </div>
  {% endfor %}
</div>

<script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d=hbglEpf0RAKZZ8FUj0xshAsymbHulHQEq7Pao7vKCf8&cl=ffffff&w=a"></script>
