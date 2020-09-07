<template>
  <div>
      <a href="https://www.google.com/webhp?hl=ja&sa=X&ved=0ahUKEwjAnv2c89PrAhXYaN4KHbcnCpYQPAgI">
        ここをクリックするとgoogle検索Topを開く
      </a>
      <p>
        pタグは段落を表現する時に使用する。<br>
      <br>
        brタグを使用することで<br>
        改行できる。<br>
        <br>
        注意点として、brタグは文頭に記載しても動作するが、原則文末に記載した方が良い。<br>
        文頭に記載しても動作するブラウザもあるかもしれないが、ブラウザは<br>
        HTML内の改行を半角スぺースに置き換える。<br> 
        そのためブラウザを表示している横幅次第では予期せぬ箇所で改行が発生してしまう可能性がある。<br>
        それを防ぐために文末に記載した方が良い。<br>
        <br>
      </p>
      <ul id = "list1">
        <li v-for = "item in itmes" :key = "item.message">
          {{ item.message }}
        </li>
      </ul>
      <ol>
        <li>ulタグ、olタグにはliタグを必ず含める</li><br>
        <li>逆に、liタグはulタグもしくはolタグで囲う</li><br>
        <li>従ってそれぞれのタグは単独で使用しない</li><br>
      </ol>
  </div>
</template>


<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
  

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
