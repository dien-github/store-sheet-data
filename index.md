---
layout: default
title: "Chào mừng đến với Website của tôi"
---

# Giới thiệu

Đây là trang chủ của website. Bạn có thể thêm nội dung giới thiệu về bản thân, dự án, hoặc blog của mình.

# Liên kết nhanh
{% include navigation.html %}

# Sheet nhạc
<div class="sheet-collection">
  {% for sheet in site.sheets %}
    <div class="sheet-item">
      <h2><a href="{{ sheet.url | relative_url }}">{{ sheet.title }}</a></h2>
      <p>Composer: {{ sheet.composer }} - Date: {{ sheet.date | date: "%d/%m/%Y" }}</p>
    </div>
  {% endfor %}
</div>
