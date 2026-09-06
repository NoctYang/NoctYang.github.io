## Publications

<p class="author-legend"><sup>*</sup> equal contribution&emsp;<sup>†</sup> project lead&emsp;<sup>‡</sup> corresponding author</p>

<div class="publication-filter">
<input class="publication-filter-input" type="radio" id="pub-filter-selected" name="pub-filter" checked>
<label class="publication-filter-label" for="pub-filter-selected">Selected</label>
<span class="publication-filter-separator">|</span>
<input class="publication-filter-input" type="radio" id="pub-filter-all" name="pub-filter">
<label class="publication-filter-label" for="pub-filter-all">All</label>

<div class="publications publication-list publication-list-selected">
<ol class="bibliography">
{% for link in site.data.publications.main %}
{% if link.selected %}
{% include publication_entry.html link=link %}
{% endif %}
{% endfor %}
</ol>
</div>

<div class="publications publication-list publication-list-all">
<ol class="bibliography">
{% for link in site.data.publications.main %}
{% include publication_entry.html link=link %}
{% endfor %}
</ol>
</div>
</div>
