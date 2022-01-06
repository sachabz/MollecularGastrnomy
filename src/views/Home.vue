<template>
  <div class="home">
    <Navbar />
    <div class="content">
      <Slogan
        class="bold"
        msg="Mollecular Gastronomy"
        msg2="Make it SIMPLE"
        auteur="By Thierry MARX"
      />
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
@import url("https://fonts.googleapis.com/css2?family=Rokkitt&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Rokkitt:wght@400;800&display=swap");
.content {
  background-image: url("../assets/fondchimievertrose.jpg");
  background-size: 100vh;
  background-repeat: no-repeat;
  font-family: "Rokkitt", serif;
}
.bold {
  font-family: "Rokkitt", serif;
  font-style: bold;
}
</style>