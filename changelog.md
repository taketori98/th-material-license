---
layout: default
nav_order: 3
has_toc: false
last_modified_date: 2026-07-27
---

# 変更履歴

{% for update in site.data.updates %}

## {{ update.date }}

<div class="changelog-item">
  {% include render_update_content.html text=update.content mode="html" %}
</div>

{% endfor %}
