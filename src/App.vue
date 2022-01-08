<template>
  <div id="nav" class="p-3">
    <router-link to="/">
      <span class="mr-3">
        <img
          src="./assets/logoMarksblanc.png"
          height="48"
          width="48"
          style="display: inline-block; vertical-align: middle"
        />
      </span>
    </router-link>
    <router-link to="/recipies" class="mr-3">Recipies.</router-link>
    <router-link to="/login" class="mr-3">Login|Register.</router-link>
    <router-link to="/register" class="mr-3">
      <span>
        <i class="far fa-user" style="display: inline-block; vertical-align: middle"></i>
      </span>
    </router-link>
  </div>

  <router-view v-slot="{ Component }">
    <transition name="route" mode="out-in">
      <component :is="Component"></component>
    </transition>
  </router-view>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Rokkitt&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Rokkitt:wght@400;800&display=swap");
#app {
  font-family: "Rokkit", serif !important;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  a {
    font-weight: bold;
    color: #ffffff;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
  background-color: rgb(0, 0, 0);
}

.route-enter-from {
  opacity: 0;
  transform: translateX(100px);
}

.route-enter-active {
  transition: all 0.3s ease-out;
}

.route-leave-to {
  opacity: 0;
  transform: translateX(-100px);
}

.route-leave-active {
  transition: all 0.3s ease-in;
}
</style>
