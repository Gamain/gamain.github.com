---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

<ul>
	{% for post in site.posts %}
		
		<li>
			<div class="article-top wordwrap"> 发表文章 </div>

			<div class="article-title">
				<a href="{{ post.url }}">{{ post.title }}</a>
			</div>
			
			<div class="article-body article-type-text clearfix">   
				<div class="article-content wordwrap"> 
				  <span class="article-text">　
					{{ post.content | strip_html | truncatewords:200  }}
				  </span> 
					<a href="{{ post.url }}" class="more-link songti">查看全文&gt;&gt;</a> 
				 </div> 
			</div>

			<div class="article-info"> 
				<a href="#"  class="repeat songti">评论</a> 
				<span class="time">{{ post.date }}</span> 
			</div>

		</li>
	{% endfor %}
</ul>

