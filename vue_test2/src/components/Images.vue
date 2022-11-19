<template>
    <div class="img">
        <img :src="link">
    </div>
</template>

<script>
export default {
  name: 'Images',
  props: {
    link: String
  }
}
</script>


<style>
.img{
    width: 50px;
    height: 50px;
    font-weight: bold;
}
</style>