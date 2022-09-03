<script src="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.js"></script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/list.js/2.3.1/list.min.js"></script>

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.css">

# Matsunotakanori.github.io
## library

<div id="books">
  <input class="search" placeholder="検索" />
  <button class="sort" data-sort="title">
    タイトルで並べ替え
  </button>
  <ul class="list">
    <!-- _data フォルダの books.csv からデータを取り出す -->
    {% for book in site.data.books %}
      <li>
        <!-- books.csv の title 列、 url 列をリンク先に設定 -->
        <p class="title"><a href="{{ book.url }}">{{ book.title }}</a></p>
      </li>
    {% endfor %}
  </ul>
</div>


<script>
var options = {
    valueNames: [ 'title' ]
};

var userList = new List('books', options);
</script>



