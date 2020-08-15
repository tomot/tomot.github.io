---
title: ToMoT - ホーム
---
### <img src="assets/images/face.png" height="60"> ToMoTのブログへようこそ！

**友達が少ない（いない？）ことに気付いてしまった大阪のおじさん**

休日出勤がやたらと多いので、平日の代休がたんまり。混んでいない平日にぶらぶらできるのは幸せだ！・・・と言いたいところだが、誰とも予定が合わないので、ますます友達ができない悪循環。

これはマズいと多趣味に走る今日この頃。ひとりでも寂しくないぞ！（と自分に言い聞かせ）

ということで、趣味の備忘録を兼ねたブログを立ち上げてみた。

ちなみ、左上の顔マークは、昔々、あるMacのOSに入っていたアイコン。おそらく20年以上前。（コピーライトについてはイマイチ分からず使っているので、もし問題があればご指摘ください。）

---

**すべての記事**

<p class="mb-1">2020年</p>
<ul class="list-unstyled ml-3 mb-1">
<li><span class="badge badge-danger">New</span> <a href="pages/motorcycle-HT2020.html">北海道ツーリング 2020</a> （2020年08月15日）</li>
<li><a href="pages/book-etc.html">読書メモ：その他</a> （2020年08月12日）</li>
<li><a href="pages/book-kishi.html">読書メモ：貴志祐介著　防犯探偵・榎本シリーズ</a> （2020年08月12日）</li>
<li><a href="pages/book-imamura.html">読書メモ：今村翔吾著　くらまし屋稼業シリーズ</a> （2020年08月12日）</li>
<li><a href="pages/book-saeki.html">読書メモ：佐伯泰英著　居眠り磐音 決定版シリーズ</a> （2020年08月01日）</li>
<li><a href="pages/camp-osaka.html">大阪のキャンプ場</a> （2020年07月20日）</li>
<li><a href="pages/book-clancy.html">読書メモ：トム・クランシー著　井坂清訳　ジャック・ライアンシリーズ</a> （2020年07月06日）</li>
<li><a href="pages/book-wakatake.html">読書メモ：若竹七海著　葉村晶シリーズ</a> （2020年07月06日）</li>
<li><a href="pages/book-konno.html">読書メモ：今野敏著　隠蔽捜査シリーズ</a> （2020年07月05日）</li>
<li><a href="pages/camp-free.html">無料のキャンプ場</a> （2020年06月14日）</li>
<li><a href="pages/camp-ownway.html">予約不要のキャンプ場</a> （2020年06月14日）</li>
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
