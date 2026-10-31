---
title: "Publications"
layout: page
permalink: /publications/
---

# Publications

<input type="text" class="pub-search" id="pubSearch" placeholder="Filter by title, author, or year...">

<div class="section-card" id="pubList">

{% capture review %}{% bibliography --query @unpublished %}{% endcapture %}
{% if review contains "pub-entry" %}
<h2>Under Review</h2>

{{ review }}
{% endif %}

{% capture conference %}{% bibliography --query @inproceedings %}{% endcapture %}
{% if conference contains "pub-entry" %}
<h2>Conference Proceedings</h2>

{{ conference }}
{% endif %}

</div>
