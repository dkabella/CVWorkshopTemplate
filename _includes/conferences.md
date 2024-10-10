<h2 id="publications" style="margin: 2px 0px -15px;">Conferences & Invited Talks</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.pubscombined.main %}
{% if link.type contains "conference" %}

<li>
<div class="pub-row">
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.text }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="periodical"><em>{{ link.conference }}, {{ link.date }}</em>
      </div>
    <div class="links">
      {% if link.text %} 
      <a href="{{ link.text }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Link</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.notes %} 
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>
{% endif %}
{% endfor %}

</ol>
</div>
