---
layout: page
title: Publications
permalink: /publications/
---

{% assign sorted_pubs = site.data.publications %}
{% for pub in sorted_pubs %}
- **{{ pub.authors }}** ({{ pub.year }}). *{{ pub.title }}*. _{{ pub.journal }}_. {% if pub.url %}[PDF]({{ pub.url }}){% endif %}
{% endfor %}
