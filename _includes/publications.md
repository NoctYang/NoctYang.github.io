## Publications

<p class="author-legend">* equal contribution&emsp;† corresponding author&emsp;‡ corresponding author</p>

<fieldset class="publication-filter">
<legend class="publication-filter-legend">Show publications</legend>
<input class="publication-filter-input" type="radio" id="pub-filter-selected" name="pub-filter" value="selected" aria-controls="publication-list-selected" checked>
<label class="publication-filter-label" for="pub-filter-selected">Selected</label>
<span class="publication-filter-separator" aria-hidden="true">/</span>
<input class="publication-filter-input" type="radio" id="pub-filter-all" name="pub-filter" value="all" aria-controls="publication-list-all">
<label class="publication-filter-label" for="pub-filter-all">All</label>

<div class="publications publication-list publication-list-selected" id="publication-list-selected">
<ol class="bibliography">
{% for link in site.data.publications.main %}
{% if link.selected %}
{% include publication_entry.html link=link %}
{% endif %}
{% endfor %}
</ol>
</div>

<div class="publications publication-list publication-list-all" id="publication-list-all">
<ol class="bibliography">
{% for link in site.data.publications.main %}
{% include publication_entry.html link=link %}
{% endfor %}
</ol>
</div>
</fieldset>
