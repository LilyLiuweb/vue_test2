<template>
<header>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">about</router-link> |
    <router-link to="/news">news</router-link> |
    <router-link to="/product">product</router-link>
  </nav>
</header>
  <router-view/>
  <footer>footer</footer>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
*{
  margin: 0;
  padding: 0;
}
header{
  background-color: #fa0;
}
footer{
  background-color: #2c3e50;
  line-height: 5rem;
  color: #ddd;
}
main{
  font-size: 5rem;
  line-height: 100vh;
  background-color: #ddd;;
}
nav {
  padding: 30px;
  router-link{
      padding: 1rem;
  }
  a {
    font-weight: bold;
    color: #2c3e50;
    
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
