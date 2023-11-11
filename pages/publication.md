---

layout: page

show\_meta: false

title: "Publication"

subheadline: ""

teaser: 

header:

   image\_fullwidth: 

permalink: "/publication/"

---

<!-- [[2021][1]] [[2020][2]] [[2019][3]] [[2018][4]] [[2017][5]] [[2016][6]] -->

<div class="">

    {% assign publications = site.publications | sort: "date" | reverse %}
    {% for pub in publications %}

        {%  include pub_item.html 
            
            title=pub.title
            author_list=pub.author_list
            pub_in=pub.pub_in
            bib=pub.bib
            grant=pub.grant
            img_path1=pub.img_path1
            img_path2=pub.img_path2
            pdf_url=pub.pdf_url
            website=pub.website
            code_url=pub.code_url
            blog_post=pub.blog_post
            oral=pub.oral
            
        %}    


    {% endfor %}


</div>


[1]:	/publication/#2021
[2]:	/publication/#2020
[3]:	/publication/#2019
[4]:    /publication/#2018
[5]:    /publication/#2017
[6]:    /publication/#2016