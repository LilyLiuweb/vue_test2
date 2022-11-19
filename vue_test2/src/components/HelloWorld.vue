<template>
  <div class="hello">
    <div class="img" v-for="item in 6" :key="item">
      <img :src="require(`@/assets/avatar/sub${item}.png`)" alt="">
      <h1>{{title}}</h1>
      <h3>{{msg}}</h3>
      <p>{{content}}</p>
      <button>go shopping</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    title :String,
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.hello{
  width: 100%;
  height: 300px;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  background-color: #ccc;
}
h1 {
  font-size: 2rem;
}
h3 {
  margin: 10px 0 0;
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
.img{
  width: 100px;
}
.img img{
  width: 100%;
}
</style>
