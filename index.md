---
layout: page
title: 
tagline: 纸上得来终觉浅，绝知此事要躬行。
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
					{{ post.content | strip_html | slice:200 }}
				  </span> 
					<a href="{{ post.url }}" class="more-link songti">查看全文&gt;&gt;</a> 
				 </div> 
			</div>

			<div class="article-info"> 
				<a href="{{ post.url }}#comments"  class="repeat songti">评论</a> 
				<span class="time">{{ post.date }}</span> 
			</div>

		<hr style="border-top:1px dashed #cccccc; height:1px">
		</li>
	{% endfor %}
</ul>

