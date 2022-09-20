<script src="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/list.js/2.3.1/list.min.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.css">

## Matsunotakanori.github.io/sharoshi_low
ver 0.1

#　社会保険労務士法　2022−09−20



<div id="rouki_souran_up">
  <input class="search" placeholder="検索" />

 <button class="sort" data-sort="t1">
    掲載順
  </button>

  
  <ul class="list">
    <!-- _data フォルダの rouki_souran_up.csv からデータを取り出す -->
    {% for komoku in site.data.sharoshi_low. %}
      <li>
        <!-- books.csv の title 列、 url 列をリンク先に設定 -->
        <p class="t2">{{ komoku.t1 }}　&nbsp;{{ komoku.t2 }}&nbsp;{{ komoku.t3 }}</p>
      </li>
    {% endfor %}
  </ul>
</div>

<script>
var options = {
    valueNames: [ 't2' ]
};

var userList = new List('sharoshi_low', options);
</script>

