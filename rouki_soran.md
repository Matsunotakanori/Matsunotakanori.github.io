<script src="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/list.js/2.3.1/list.min.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.css">

## Matsunotakanori.github.io/rouki_soran

<div id="books">
  <input class="search" placeholder="検索" />
  <button class="sort" data-sort="t1">
    タイトルで並べ替え
  </button>
  <ul class="list">
    <!-- _data フォルダの books.csv からデータを取り出す -->
    <!-- _data フォルダの rouki_soran.csv からデータを取り出す -->
    {% for data in site.data.rouki_soran %}
      <li>
        <!-- books.csv の title 列、 url 列をリンク先に設定 -->
        <p class="t6">{{ book.t6 }}</p>
      </li>
    {% endfor %}
  </ul>
</div>

<script>
var options = {
    valueNames: [ 't1' ]
};

var userList = new List('rouki_soran', options);
</script>

