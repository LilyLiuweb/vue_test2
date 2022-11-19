<template>
  <div class="home">
    <HelloWorld title="title1" msg="1"/>
    <HelloWorld title="title2" msg="2"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Images from '@/components/Images.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    Images
  }
}
</script>
<style>
.img img{
  width: 60px;
  height: 60px;
}
</style>