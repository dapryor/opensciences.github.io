---
title: Data Categories
layout: repo-content
custom_js:
- jquery.min
- jquery-maxHeight
---
<head>
	{% if page.custom_js %}
  		{% for js_file in page.custom_js %}
  			<script src='/javascripts/{{ js_file }}.js' type="text/javascript"></script>
  		{% endfor %}
	{% endif %}
</head>
This is a listing of all dataset categories currently being maintained on tera-PROMISE. Check out the brief descriptions of each category to find what you're looking for.

**Note:** Category descriptions are under construction as of May 11th.

{% for category in site.datacategories %}
<div class="categories col-lg-3 col-md-4 col-sm-6 col-xs-6">
<a href="{{category.repourl}}">
<div class="well">
<h3 class="page-header">{{category.title}}</h3>
</div>
</a>
</div>
{% endfor %}
