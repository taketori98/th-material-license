---
layout: default
nav_order: 3
has_toc: false
last_modified_date: 2026-07-27
---

# 変更履歴

## RSSについて

更新情報はRSSでも配信しています。

RSSリーダーや[SlackのRSSアプリ](https://slack.com/intl/ja-jp/help/articles/218688467-Slack-%E3%81%AB-RSS-%E3%83%95%E3%82%A3%E3%83%BC%E3%83%89%E3%82%92%E8%BF%BD%E5%8A%A0%E3%81%99%E3%82%8B)に以下のURLを設定することで、更新があった際に逐次情報を受け取ることが可能です。

<a href="{{ "/feed.xml" | absolute_url }}">
{{ "/feed.xml" | absolute_url }}
</a>

{% for update in site.data.updates %}

## {{ update.date }}

<div class="changelog-item">
  {% include render_update_content.html text=update.content mode="html" %}
</div>

{% endfor %}
