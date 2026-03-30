<h2 id="publications" style="margin-bottom: 20px;">Publications</h2>

<h4 style="margin:0 10px 10px;">Journal Papers:</h4>
<div class="publications">
  <ol class="bibliography" style="list-style: none; padding-left: 0;">
    {% for entry in site.data.publications.journals %}
    <li style="margin-bottom: 25px;">
      <div class="row" style="display: flex;">
        <div class="col-sm-10" style="flex: 0 0 85%;">
          <span class="authors">{{ entry.authors }}.</span> 
          <span class="year">({{ entry.year }}).</span> 
          <span class="title" style="font-weight: bold;">{{ entry.title }}.</span> 
          <span class="periodical" style="font-style: italic;">{{ entry.journal }}</span>{% if entry.volume %}, <span>{{ entry.volume }}</span>{% if entry.number %}({{ entry.number }}){% endif %}{% endif %}{% if entry.pages %}, {{ entry.pages }}{% endif %}.
          {% if entry.doi %}
          <div class="doi" style="font-size: 0.9rem; color: #666;">
            DOI: <a href="https://doi.org/{{ entry.doi }}" target="_blank">https://doi.org/{{ entry.doi }}</a>
          </div>
          {% endif %}
          <div class="links" style="margin-top: 8px;">
            {% if entry.url %}<a href="{{ entry.url }}" class="btn btn-sm" style="border: 1px solid #ddd; padding: 2px 8px; font-size: 0.8rem; text-decoration: none; color: #333;">Link</a>{% endif %}
            {% if entry.pdf %}<a href="{{ entry.pdf }}" class="btn btn-sm" style="border: 1px solid #ddd; padding: 2px 8px; font-size: 0.8rem; text-decoration: none; color: #333;">PDF</a>{% endif %}
          </div>
        </div>
      </div>
    </li>
    {% endfor %}
  </ol>
</div>

<h4 style="margin:20px 10px 10px;">Conference Papers:</h4>
<div class="publications">
  <ol class="bibliography" style="list-style: none; padding-left: 0;">
    {% for entry in site.data.publications.conferences %}
    <li style="margin-bottom: 25px;">
      <div class="row" style="display: flex;">
        <div class="col-sm-10" style="flex: 0 0 85%;">
          <span class="authors">{{ entry.authors }}.</span> 
          <span class="year">({{ entry.year }}).</span> 
          <span class="title" style="font-weight: bold;">{{ entry.title }}.</span> 
          In <span class="periodical" style="font-style: italic;">{{ entry.booktitle }}</span>{% if entry.pages %}, (pp. {{ entry.pages }}){% endif %}. {{ entry.address }}.      
          {% if entry.doi %}
          <div class="doi" style="font-size: 0.9rem; color: #666;">
            DOI: <a href="https://doi.org/{{ entry.doi }}" target="_blank">https://doi.org/{{ entry.doi }}</a>
          </div>
          {% endif %}
          <div class="links" style="margin-top: 8px;">
            {% if entry.url %}<a href="{{ entry.url }}" class="btn btn-sm" style="border: 1px solid #ddd; padding: 2px 8px; font-size: 0.8rem; text-decoration: none; color: #333;">Link</a>{% endif %}
          </div>
        </div>
      </div>
    </li>
    {% endfor %}
  </ol>
</div>
