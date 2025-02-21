---
# Mr. Green Jekyll Theme - v1.1.0 (https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme)
# Copyright (c) 2022 Mr. Green's Workshop https://www.MrGreensWorkshop.com
# Licensed under MIT

layout: default
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}
{%- include post_common/post-main.html post = page -%}

{%-comment-%} Pagination {%-endcomment-%}


{% if site.data.conf.posts.comments.enable and site.data.conf.posts.comments.disqus.enable and page.comments_disable != true %}
  {% include post/disqus.html %}
{% endif %}
