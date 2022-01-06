<template>
  <div id="nav"></div>
  <router-view />
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Rokkitt&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Rokkitt:wght@400;800&display=swap");
#app {
  font-family: "Rokkit", Helvetica, Arial, serif !important;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
