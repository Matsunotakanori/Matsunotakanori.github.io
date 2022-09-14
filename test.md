
ver 1.1
<div>
  <ul>
    <!-- _data フォルダの books.csv からデータを取り出す -->
    {% for book in site.data.rouki_souran_up %}
    
      <li>
        <!-- books.csv の title 列を表示、 url 列をリンク先に設定 -->
        <p class="t1">{{ book.t1 }} {{ book.2 }}</p>
      </li>
    {% endfor %}
  </ul>
</div>


