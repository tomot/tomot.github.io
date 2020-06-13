---
title: ToMoT - ホーム
---
### <img src="assets/images/face.png" height="60"> ToMoTのブログへようこそ！

**友達が少ない（いない？）ことに気付いてしまった大阪のおじさん**

休日出勤がやたらと多いので、平日の代休がたんまり。混んでいない平日にぶらぶらできるのは幸せだ！・・・と言いたいところだが、誰とも予定が合わないので、ますます友達ができない悪循環。

これはマズいと多趣味に走る今日この頃。ひとりでも寂しくないぞ！（と自分に言い聞かせ）

ということで、趣味の備忘録を兼ねたブログを立ち上げてみた。

ちなみ、左上の顔マークは、昔々、あるMacのOSに入っていたアイコン。おそらく20年以上前。（コピーライトについてはイマイチ分からず使っているので、もし問題があればご指摘ください。）

<ul class="nav nav-tabs mb-2">
  <li class="nav-item">
    <a class="nav-link active" data-toggle="tab" href="#latest-post" aria-controls="latest-post" aria-selected="true">最近の記事</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" data-toggle="tab" href="#all-post" aria-controls="all-post" aria-selected="false">すべての記事</a>
  </li>
</ul>
<div class="tab-content">
  <div class="tab-pane fade show active" id="latest-post">
    <ul class="list-unstyled ml-3">
      <li><a href="pages/camp-osaka.html">大阪のキャンプ場</a> （2020年06月14日）</li>
      <li><a href="pages/camp-free.html">無料のキャンプ場</a> （2020年06月14日）</li>
      <li><a href="pages/camp-ownway.html">予約不要のキャンプ場</a> （2020年06月14日）</li>
      <li><a href="pages/book-konno.html">今野敏著　隠蔽捜査シリーズ</a> （2020年06月13日）</li>
    </ul>
    <ul class="list-unstyled ml-3 mb-1">
      {% for post in site.posts limit: site.latestPosts %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a>
          （{{ post.date | date: "%Y年%m月%d日" }}）
        </li>
      {% endfor %}
    </ul>
  </div>
  <div class="tab-pane fade" id="all-post">
    <p class="mb-1">2020年</p>
    <ul class="list-unstyled ml-3">
      <li><a href="pages/camp-osaka.html">大阪のキャンプ場</a> （2020年06月14日）</li>
      <li><a href="pages/camp-free.html">無料のキャンプ場</a> （2020年06月14日）</li>
      <li><a href="pages/camp-ownway.html">予約不要のキャンプ場</a> （2020年06月14日）</li>
      <li><a href="pages/book-konno.html">今野敏著　隠蔽捜査シリーズ</a> （2020年06月13日）</li>
    </ul>
    <p class="mb-1">2019年</p>
    <ul class="list-unstyled ml-3 mb-1">
      {% for post in site.posts %}
        {% capture year %}{{ post.date | date: "%Y" }}{% endcapture %}
        {% if year == "2019" %}
          <li>
            <a href="{{ post.url }}">{{ post.title }}</a>
            （{{ post.date | date: "%Y年%m月%d日" }}）
          </li>
        {% endif %}
      {% endfor %}
    </ul>

    <p class="mb-1">2018年</p>
    <ul class="list-unstyled ml-3 mb-1">
      {% for post in site.posts %}
        {% capture year %}{{ post.date | date: "%Y" }}{% endcapture %}
        {% if year == "2018" %}
          <li>
            <a href="{{ post.url }}">{{ post.title }}</a>
            （{{ post.date | date: "%Y年%m月%d日" }}）
          </li>
        {% endif %}
      {% endfor %}
    </ul>

    <p class="mb-1">2017年</p>
    <ul class="list-unstyled ml-3 mb-1">
      {% for post in site.posts %}
        {% capture year %}{{ post.date | date: "%Y" }}{% endcapture %}
        {% if year == "2017" %}
          <li>
            <a href="{{ post.url }}">{{ post.title }}</a>
            （{{ post.date | date: "%Y年%m月%d日" }}）
          </li>
        {% endif %}
      {% endfor %}
    </ul>
  </div>
</div>
