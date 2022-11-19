<template>
  <div class="news">
    <h1>This is an news page</h1>
    <HelloWorld title="我是最新消息"></HelloWorld>
    <Images link="https://picsum.photos/300/200/?random=15"></Images>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Images from '@/components/Images.vue'

export default {
  name: 'NewsView',
  components: {
    HelloWorld,
    Images
  }
}
</script>
<style>
.news{
  text-align: center;
  padding: 1rem;
  background-color: pink;
}
</style>