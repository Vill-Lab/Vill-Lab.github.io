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

	<h3 class="section-title">Principal Investigator</h3>

    {% include member.html 
   
   		name="Cairong Zhao" 
   		title="Professor" 
   		<!-- photo="/images/people/LiZhang.jpg"  -->
   		website="http://www.baidu.com" 
   		google="https://baidu.com" 
   		email="test@tongji.edu.cn"
   
   	%}
	
	<hr/>

	<h3 class="medium-12 section-title">PhD Students</h3>

	{% for a in site.phd %}
		{% include collaborator.html 
            name=a.name 
            title=a.title 
            email=a.email 
            website=a.website 
            note=a.note 
        %}
	{% endfor %}

	<hr/>

	<h3 class="medium-12 section-title">Master Students</h3>

	{% for a in site.master %}
		{% include collaborator.html 
            name=a.name 
            title=a.title 
            email=a.email 
            website=a.website 
            note=a.note 
		%}
	{% endfor %}

	<hr/>

	<h3 class="medium-12 section-title">Visiting Students</h3>

	{% for a in site.visit %}
		{% include collaborator.html 
            name=a.name 
            title=a.title 
            email=a.email 
            website=a.website 
            note=a.note 
		%}
	{% endfor %}

	<hr/>

</div>




