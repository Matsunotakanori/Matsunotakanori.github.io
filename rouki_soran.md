<script src="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/list.js/2.3.1/list.min.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.css">

## Matsunotakanori.github.io/rouki_soran

ver 1.8

<a href = "https://iss.ndl.go.jp/books/R100000002-I025614893-00">労働基準法解釈総覧　第15版</a>



<div id="rouki_souran_up">
  <input class="search" placeholder="検索" />
  <button class="sort" data-sort="t1">
    ページ順
  </button>
  <ul class="list">
    <!-- _data フォルダの rouki_souran_up.csv からデータを取り出す -->
    {% for mokuji in site.data.rouki_souran_up %}
      <li>
        <!-- books.csv の title 列、 url 列をリンク先に設定 -->
        <p class="t6">No.{{ mokuji.t1 }}_{{ mokuji.t2 }}_{{ mokuji.t3 }}_{{ mokuji.t4 }}_{{ mokuji.t5 }}_{{ mokuji.t6 }}_{{ mokuji.t7 }}</p>
      </li>
    {% endfor %}
  </ul>
</div>

<script>
var options = {
    valueNames: [ 't6' ]
};

var userList = new List('rouki_souran_up', options);
</script>

