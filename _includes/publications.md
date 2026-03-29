## Publications

<h2 id="publications" style="margin-bottom: 20px;">Publications</h2>

<h3 style="font-size: 1.2rem; border-bottom: 1px solid #eee; padding-bottom: 5px;">Journal Papers</h3>
<div class="publications">
<ol class="bibliography" style="list-style: none; padding-left: 0;">
{% for link in site.data.publications.journals %}
  <li style="margin-bottom: 25px;">
    <div class="row" style="display: flex;">
      <div class="col-sm-2" style="flex: 0 0 15%; padding-right: 10px;">
        {% if link.image %}<img src="{{ link.image }}" style="width: 100%; border-radius: 4px; box-shadow: 0 2px 5px rgba(0,0,0,0.1);">{% endif %}
      </div>
      <div class="col-sm-10" style="flex: 0 0 85%;">
        <span class="author">{{ link.authors }}</span> 
        <span class="year">({{ link.year }}).</span> 
        <span class="title" style="font-weight: bold;">{{ link.title }}.</span> 
        <span class="periodical" style="font-style: italic;">{{ link.conference }}.</span>
        {% if link.doi %}<span class="doi">https://doi.org/{{ link.doi }}</span>{% endif %}
        
        <div class="links" style="margin-top: 8px;">
          {% if link.pdf %}<a href="{{ link.pdf }}" class="btn btn-sm" style="border: 1px solid #ddd; padding: 2px 8px; font-size: 0.8rem;">PDF</a>{% endif %}
          {% if link.code %}<a href="{{ link.code }}" class="btn btn-sm" style="border: 1px solid #ddd; padding: 2px 8px; font-size: 0.8rem;">Code</a>{% endif %}
        </div>
      </div>
    </div>
  </li>
{% endfor %}
</ol>
</div>

<h3 style="font-size: 1.2rem; border-bottom: 1px solid #eee; padding-bottom: 5px; margin-top: 40px;">Conference Papers</h3>
<div class="publications">
<ol class="bibliography" style="list-style: none; padding-left: 0;">
{% for link in site.data.publications.conferences %}
  <li style="margin-bottom: 25px;">
    <div class="row" style="display: flex;">
      <div class="col-sm-2" style="flex: 0 0 15%; padding-right: 10px;">
        {% if link.image %}<img src="{{ link.image }}" style="width: 100%; border-radius: 4px;">{% endif %}
      </div>
      <div class="col-sm-10" style="flex: 0 0 85%;">
        <span class="author">{{ link.authors }}</span> 
        <span class="year">({{ link.year }}).</span> 
        <span class="title" style="font-weight: bold;">{{ link.title }}.</span> 
        In <span class="periodical" style="font-style: italic;">{{ link.conference }}</span>.
        
        <div class="links" style="margin-top: 8px;">
          {% if link.pdf %}<a href="{{ link.pdf }}" class="btn btn-sm" style="border: 1px solid #ddd; padding: 2px 8px; font-size: 0.8rem;">PDF</a>{% endif %}
        </div>
      </div>
    </div>
  </li>
{% endfor %}
</ol>
</div>
