## Publications
<h4 style="margin:0 10px 0;">Selected Journal Papers</h4>
<div class="publications">
<ol class="bibliography">
{% for link in site.data.publications.journals %}
<li>
<div class="pub-row">
{% if link.image %}
<img src="{{ link.image }}" class="teaser img-fluid" style="width:100px; margin-right:10px;">
{% if link.conference_short %} <abbr class="badge">{{ link.conference_short }}</abbr> {% endif %}
{% endif %}

<div class="title"><strong>{{ link.title }}</strong></div>
<div class="author">{{ link.authors }}</div>
<div class="periodical"><em>{{ link.conference }}</em></div>

<div class="links">
  {% if link.pdf %} <a href="{{ link.pdf }}" class="btn btn-sm">PDF</a> {% endif %} 
  {% if link.code %} <a href="{{ link.code }}" class="btn btn-sm">Code</a> {% endif %} 
  {% if link.bibtex %} <a href="{{ link.bibtex }}" class="btn btn-sm">BibTex</a> {% endif %}
  {% if link.notes %} <i style="color:#e74d3c">{{ link.notes }}</i> {% endif %}
</div>
</div>
</li>


{% endfor %}
</ol>
</div>

<h4 style="margin:0 10px 0;">Conference Papers</h4>
<div class="publications">
<ol class="bibliography">
{% for link in site.data.publications.conferences %}
<li>
<div class="pub-row">
{% if link.image %}
<img src="{{ link.image }}" class="teaser img-fluid" style="width:100px; margin-right:10px;">
{% if link.conference_short %} <abbr class="badge">{{ link.conference_short }}</abbr> {% endif %}
{% endif %}

<div class="title"><strong>{{ link.title }}</strong></div>
<div class="author">{{ link.authors }}</div>
<div class="periodical"><em>{{ link.conference }}</em></div>

<div class="links">
  {% if link.pdf %} <a href="{{ link.pdf }}" class="btn btn-sm">PDF</a> {% endif %} 
  {% if link.code %} <a href="{{ link.code }}" class="btn btn-sm">Code</a> {% endif %}
  {% if link.bibtex %} <a href="{{ link.bibtex }}" class="btn btn-sm">BibTex</a> {% endif %}
</div>
</div>
</li>


{% endfor %}
</ol>
</div>
