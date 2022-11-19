<template>
  <div class="about">
    <h1>This is an about page</h1>

    <Switch v-model="value1" @on-change="change" />
      <Carousel v-model="value" loop>
        <CarouselItem v-for="item in 6" :key="item">
           <div class="demo-carousel"> 
              <img :src="require(`@/assets/avatar/sub${item}.png`)" alt="">
          </div>
        </CarouselItem>
      </Carousel>
  </div>

  
</template>


<script>
    export default {
        data () {
            return {
                value1: false,
                value: 0
            }
        }
    }
</script>