---

layout: frontpage
header:
  image_fullwidth:
title: "Zhang Vision Group - Fudan University"

sidebar: right

permalink: /index.html
homepage: true

---

<div class="row" style= "margin-top: 30px; max-height: 540px; margin-left: 1%">
    <div class="light-section mt-6 mb-6">
      <h3 class="section-title">Breaking News</h3>
      <ul class="timeline col-md-6 off-md-6">
        {% for n in site.news %}
          {% include news_item.html 
              news_date=n.news_date 
              title=n.title 
              year=n.year 
              news_content=n.news_content 
              link=n.link 
              link2=n.link2
              link3=n.link3
              link4=n.link4
              link5=n.link5
          %}
        {% endfor %}
      </ul>
  </div>
</div>

<div class="pc dark-section" style="">
  <br>
  <h3 class="section-title"> Join the Group </h3> 
  
  <p>We are currently looking to hire talented students/postdoc.
  <br>
  If you are highly creative, have top grades/coding skill and interested in joining our group please do not hesitate to send your CV and transcripts of grades to <a href="mailto:test@tongji.edu.cn">test@tongji.edu.cn </a></p>
  

</div>
