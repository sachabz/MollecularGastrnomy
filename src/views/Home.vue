<template>
  <div class="home">
    <Navbar />
    <div class="content">
      <Slogan class="text-bold" auteur="By Thierry MARX">
        Mollecular Gastronomy
        <template v-slot:subtitle>
          Make it
          <span class="text-purple">SIMPLE</span>
        </template>
      </Slogan>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Navbar from '@/components/Navbar.vue'
import Slogan from '@/components/Slogan.vue'

export default {
  name: 'Home',
  components: {
    Navbar,
    Slogan
  }
}
</script>
<style scoped lang="scss">
.home {
  background-image: url("../assets/fondchimievertrose.jpg");
  height: 100vh;
  background-repeat: no-repeat;
  background-size: cover;
}
.text-bold {
  font-style: bold;
}

.text-purple {
  color: #b960ff;
}
</style>