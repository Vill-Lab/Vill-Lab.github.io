---
layout: page
show_meta: false
title: "People"
subheadline: ""
teaser: 
header:
   image_fullwidth: 
permalink: "/people/"


---

<div class="row"> 

	<hr/>

	<h2 class="section-title">Principal Investigator</h2>

	{% assign url = site.url %}
    {% include member.html 
   
   		name="Cairong Zhao" 
   		title="Professor" 
   		photo="/images/people/cairongZhao.jpg" 
   		website=url
   		google="https://scholar.google.com.hk/citations?user=z-XzWZcAAAAJ&hl=zh-CN" 
   		email="zhaocairong@tongji.edu.cn"
   
   	%}
	
	<hr/>

	<h2 class="medium-12 section-title">Enrolled Student</h2>

	<h3 class="medium-12 section-title">PhD Students</h3>

	{% assign phd = site.phd | sort: "date"  %}
	{% for a in phd %}
		{% include member.html 
            name=a.name 
            email=a.email 
            website=a.website 
            note=a.note 
			photo=a.photo
			title = a.title
        %}
		<hr/>
	{% endfor %}


	<h3 class="medium-12 section-title">Master Students</h3>
	{% assign master = site.master | sort: "date"  %}
	{% for a in master %}
		{% include member.html 
            name=a.name 
            email=a.email 
            website=a.website 
            note=a.note 
			photo=a.photo
			title = a.title 
		%}
		<hr/>
	{% endfor %}

	<hr/>

	<h2 class="medium-12 section-title">Graduated Students</h2>
	{% assign graduated = site.graduated | sort: "date"  %}
	{% for a in graduated %}	
		{% include member.html 
            name=a.name 
            email=a.email 
            website=a.website 
            note=a.note 
			photo=a.photo
			title = a.title 
		%}
		<hr/>
	{% endfor %}

</div>




