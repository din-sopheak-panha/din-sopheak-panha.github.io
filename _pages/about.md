---
title: "About"
layout: page
permalink: /about/
---

# About

<div class="section-card">
<div class="pi-card">
<img src="{{ site.photo | prepend: '/images/' | relative_url }}" class="pi-photo" alt="{{ site.name }}" width="160" height="160">
<div>
<h2 class="pi-name">{{ site.name }}</h2>
<p style="font-style: italic; color: var(--text-secondary);">{{ site.title }}, {{ site.institution }}</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email" aria-label="Email">{% include icon.html name="envelope" %}</a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{{ site.links.cv | prepend: '/' | relative_url }}" class="icon-link" title="CV" aria-label="CV">{% include icon.html name="cv" %}</a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar" aria-label="Google Scholar">{% include icon.html name="google-scholar" %}</a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub" aria-label="GitHub">{% include icon.html name="github" %}</a>{% endif %}
{% if site.links.researchgate and site.links.researchgate != "" %}<a href="{{ site.links.researchgate }}" class="icon-link" title="ResearchGate" aria-label="ResearchGate">{% include icon.html name="researchgate" %}</a>{% endif %}
{% if site.links.linkedin and site.links.linkedin != "" %}<a href="{{ site.links.linkedin }}" class="icon-link" title="LinkedIn" aria-label="LinkedIn">{% include icon.html name="linkedin" %}</a>{% endif %}
</div>
{% if site.data.pi[0].education %}
<ul style="margin-top: var(--space-4);">
{% for education in site.data.pi[0].education %}
<li>{{ education | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
{% endif %}
</div>
</div>
</div>

<div class="section-card" markdown="0">
<h3>Competitions, Leadership &amp; Memberships</h3>
<ul>
<li><b>2026-Present</b>, Member, Union of Youth Federations of Cambodia (UYFC)</li>
<li><b>2025</b>, Team Leader, ITC01, ABU Robocon 2025, GEE Lab (Electronics Engineering Lab), Institute of Technology of Cambodia.</li>
<li><b>2024</b>, Electronics Team Member, ITC02, ABU Robocon 2024, Dynamics and Control Laboratory (DCLab), Institute of Technology of Cambodia.</li>
<li><b>2023-Present</b>, Member, Dynamics and Control Laboratory (DCLab)</li>
</ul>
</div>
