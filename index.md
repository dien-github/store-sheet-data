---
layout: default
title: "Chào mừng đến với Website của tôi"
---

# Giới thiệu

Đây là trang chủ của website. Bạn có thể thêm nội dung giới thiệu về bản thân, dự án, hoặc blog của mình.

# Liên kết nhanh
- [Trang chủ](/index.md)
- [Giới thiệu thêm về tôi](/about.md)
- [Xem các bài viết trên Blog](/blog/)

# Sheet nhạc
{% for sheet in site.sheets %}
  <div class="sheet-item">
    <h2><a href="{{ sheet.url }}">{{ sheet.title }}</a></h2>
    <p>Composer: {{ sheet.composer }} - Date: {{ sheet.date | date: "%d/%m/%Y" }}</p>
  </div>
{% endfor %}
