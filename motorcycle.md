---
title: ToMoT - バイク
---
### <img src="assets/images/face.png" height="60"> 徒然バイク日記

**金なし、テクなし、根性なし、さらに仲間なしライダーの奮闘記**

愛車SR400を中心としたバイクやツーリング、グッズなどの話しを徒然なるままに書き残す。

<ul class="nav nav-tabs mb-2">
  <li class="nav-item">
    <a class="nav-link active" data-toggle="tab" href="#post" aria-controls="post" aria-selected="true">記事</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" data-toggle="tab" href="#podcast" aria-controls="podcast" aria-selected="false">Podcast</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" data-toggle="tab" href="#youtube" aria-controls="youtube" aria-selected="false">YouTube</a>
  </li>
</ul>
<div class="tab-content">
  <div class="tab-pane fade show active" id="post">
    {% for category in site.categories %}
      {% if category[0] == "バイク" %}
        <ul class="list-unstyled ml-3">
          {% for post in category[1] %}
            <li>
              <a href="{{ post.url }}">{{ post.title }}</a>
              （{{ post.date | date: "%Y年%m月%d日" }}）
            </li>
          {% endfor %}
        </ul>
      {% endif %}
    {% endfor %}
  </div>
  <div class="tab-pane fade" id="podcast">
    <ul class="list-unstyled ml-3">
      <li>
        <a href="https://podcasts.apple.com/jp/podcast/%E3%83%8A%E3%82%AB%E3%83%A4%E3%83%9E-%E3%83%90%E3%82%A4%E3%82%AF%E3%83%A9%E3%82%B8%E3%82%AA/id612297656">ナカヤマ バイクラジオ</a>
        （紹介記事は<a href="/posts/20170405a.html">こちら</a>）
      </li>
    </ul>
  </div>
  <div class="tab-pane fade" id="youtube">
    <p class="ml-3">Coming soon</p>
  </div>
</div>
