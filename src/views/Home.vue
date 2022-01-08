<template>
  <div class="home">
    <transition appear @before-enter="beforeEnter" @enter="enter">
      <div class="content">
        <Slogan class="text-bold" auteur="By Thierry MARX">
          Mollecular Gastronomy
          <template v-slot:subtitle>
            Make it
            <span class="text-purple">SIMPLE</span>
          </template>
        </Slogan>
      </div>
    </transition>
  </div>
</template>

<script>
// @ is an alias to /src

import Slogan from '@/components/Slogan.vue'
import gsap from 'gsap'

export default {
  name: 'Home',
  components: {
    Slogan
  },
  setup() {
    const beforeEnter = (el) => {
      console.log("before enter - set initial state")
      el.style.transform = 'translateY(-60px)'
      el.style.opacity = 0
    }
    const enter = (el) => {
      console.log("starting")
      gsap.to(el, { duration: 1, y: 0, opacity: 1, ease: "bounce.out" });
    }
    return { beforeEnter, enter }
  }
}
</script>
<style scoped lang="scss">
.home {
  background-image: url("../assets/fondchimievertrose.jpg");
  height: 100vh;
  background-repeat: no-repeat;
  background-size: cover;
  padding-top: 8rem;
}
.text-bold {
  font-style: bold;
}

.text-purple {
  color: #b960ff;
}
</style>