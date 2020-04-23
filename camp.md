---
title: ToMoT - キャンプ
---
### <img src="assets/images/face.png" height="60"> ひとりぼっちのキャンプ日記

**ソロキャンパーを目指しているわけではなく、誰とも予定が合わないだけ・・・**

予約不要でふらっといけるキャンプ場、無料（だけど高速代はかかる）キャンプ場、ここってホントにキャンプ場？ってな感じのキャンプ場、買い出しならここがオススメなどの備忘録。

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
      {% if category[0] == "キャンプ" %}
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
