---
layout: page
permalink: /
title: about
nav: about
---

<div class="text-center mt-5">
  <img class="profile-img" src="{{ 'prof_pic.jpg' | prepend: '/assets/img/' | prepend: site.baseurl }}">
</div>

<div class="col mt-4">
  <h1 class="title text-center font-weight-bold">Yoontae Hwang</h1>
  <div class="row mt-3 mb-3">
    <div class="col-sm-6">
      <h6 class="mt-1 text-left text-sm-right" style="font-stretch: ultra-condensed;">
        <a style="color: rgb(60, 72, 88);" href="https://unist-felab.notion.site/Yoontae-Hwang-9b1c43d6b1924d39a7940764fd0420b7" target="_blank">Ph.D Candidate</a><br />
        <a style="color: rgb(60, 72, 88);" href="https://ie.unist.ac.kr/eng/" target="_blank">Industrial Engineering</a><br />
        <a style="color: rgb(60, 72, 88);" href="https://www.unist.ac.kr/" target="_blank">UNIST</a>
      </h6>
    </div>
    <div class="col-sm-6">
      <h6 class="mt-1 text-left text-sm-left" style="font-stretch: ultra-condensed;">
        South Korea, KR
      </h6>
    </div>
  </div>
</div>

<!-- Introduction -->

<div class="col text-justify p-0">
I am a passionate researcher and Ph.D. candidate specializing in Artificial Intelligence (AI). With a strong background in AI, my primary goal is to contribute to the advancement of this field through my research. Currently, I am actively seeking opportunities to further expand my knowledge and expertise.
<br/><br/>
I anticipate graduating in September 2024, although the exact date is yet to be confirmed. My research interests primarily lie in the development and optimization of deep learning models. I have focused on various areas, including time-series modeling, which involves analyzing data in the temporal domain, as well as tabular data modeling, which deals with static domain information. Additionally, I have a keen interest in the concept of generalization and its applications in AI.
<br/><br/>
Throughout my academic journey, I have acquired comprehensive skills in AI research methodologies, data analysis, and model development. I am driven by a desire to explore novel approaches and push the boundaries of AI technology.
<br/><br/>
Please explore my website to learn more about my research, publications, and projects. If you are interested in collaborating or have any inquiries, feel free to reach out to me. I am always excited to connect with fellow researchers and industry professionals who share a passion for AI.

</div>

<!-- News -->
<div class="news mt-3 p-0">
  <h1 class="title mb-4 p-0">news</h1>
  {% assign news = site.news | reverse %}
  {% for item in news limit: site.news_limit %}
    <div class="row p-0">
      <div class="col-sm-2 p-0">
        <span class="badge danger-color-dark font-weight-bold text-uppercase align-middle date ml-3">
          {{ item.date | date: "%b %-d, %Y" }}
        </span>
      </div>
      <div class="col-sm-10 mt-2 mt-sm-0 ml-3 ml-md-0 p-0 font-weight-light text">
        <p>{{ item.content | remove: '<p>' | remove: '</p>' | emojify }}</p>
      </div>
    </div>
  {% endfor %}
</div>
