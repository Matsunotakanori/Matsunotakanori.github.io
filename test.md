

<div>
  <ul>
    <!-- _data フォルダの books.csv からデータを取り出す -->
    {% for book in site.data.rouki_soran_up %}
      <li>
        <!-- books.csv の title 列を表示、 url 列をリンク先に設定 -->
        <p class="t1"><a href="{{ book.url }}">{{ book.t1 }}</a></p>
      </li>
    {% endfor %}
  </ul>
</div>


