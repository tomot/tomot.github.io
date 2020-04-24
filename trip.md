---
title: ToMoT - 旅行
---
### <img src="assets/images/face.png" height="60"> 旅行？そこそこグルメな、出張旅行

**旅行？日頃はダイエット食なので、出張中くらいは許して欲しい**

旅行？少ないお小遣いを最大限に活用して、美味しいものを堪能する技を磨き中。後から思い出して、日々のダイエットのつらさを忘れるための備忘録！

<ul class="nav nav-tabs mb-2">
  <li class="nav-item">
    <a class="nav-link active" data-toggle="tab" href="#post-date" aria-controls="post-date" aria-selected="true">記事（日付）</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" data-toggle="tab" href="#post-area" aria-controls="post-area" aria-selected="false">記事（地域）</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" data-toggle="tab" href="#podcast" aria-controls="podcast" aria-selected="false">Podcast</a>
  </li>
</ul>
<div class="tab-content">
  <div class="tab-pane fade show active" id="post-date">
    <p class="mb-1">2017年</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ml-3">
          {% for post in category[1] %}
            {% capture year %}{{ post.date | date: "%Y" }}{% endcapture %}
            {% if year == "2017" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}
  </div>
  <div class="tab-pane fade" id="post-area">
    <p class="mb-0">宮城県仙台市</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ml-3">
          {% for post in category[1] %}
            {% if post.tags contains "仙台市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">東京都</p>
    <p class="mb-0 ml-3">五反田</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ml-4">
          {% for post in category[1] %}
            {% if post.tags contains "五反田" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0 ml-3">羽田空港</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ml-4">
          {% for post in category[1] %}
            {% if post.tags contains "羽田空港" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">愛媛県松山市</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ml-3">
          {% for post in category[1] %}
            {% if post.tags contains "松山市" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}

    <p class="mb-0">その他</p>
    {% for category in site.categories %}
      {% if category[0] == "旅行" %}
        <ul class="list-unstyled ml-3">
          {% for post in category[1] %}
            {% if post.tags contains "その他" %}
              <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
                （{{ post.date | date: "%Y年%m月%d日" }}）
              </li>
            {% endif %}
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}
  </div>
  <div class="tab-pane fade" id="podcast">
    <p class="ml-3">Coming soon</p>
  </div>
</div>
