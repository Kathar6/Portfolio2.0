<template>
  <!-- <div id="nav">
    
  </div> -->
  <router-view />
</template>

<style lang="scss">
* {
  margin: 0;
}
body {
  padding: 0;
  margin: 0;
  background-color: #eee;
}
#app {
  font-family: Avenir, "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
