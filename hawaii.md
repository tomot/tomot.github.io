---
title: ToMoT - ハワイ
---
### <img src="assets/images/face.png" height="60"> ハワイ生活（不安だらけの）準備日記

**2020年秋から１年間、ハワイへ出向することになった！**

新型コロナウイルスの猛威が世界中を震撼させているのに・・・

米国ビザは取得できるのか？　住むところは見つかるのか？　そもそも入国できるのか？　不安材料は多々あるが、とにかく準備を始めねば！

ということで、ハワイ生活に向けた準備の様子を日記風に記録していくページ。

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
    <p class="ml-3">Coming soon</p>
    {% for category in site.categories %}
      {% if category[0] == "ハワイ" %}
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
    <p class="ml-3">Coming soon</p>
  </div>
  <div class="tab-pane fade" id="youtube">
    <p class="ml-3">Coming soon</p>
  </div>
</div>
