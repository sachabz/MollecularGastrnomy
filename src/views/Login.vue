<template>
  <div class="home">
    <Navbar />
    <div class="content">
      <Title title="Login" />
      <Inputpage nameinput="Email : " />
      <Inputpwd nameinput="Password : " />
      <Buttonsubmit textbutton="Submit" />
      <router-link to="/register">
        <p class="text-green mt-4">Not already a member, click here.</p>
      </router-link>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Navbar from '@/components/Navbar.vue'
import Title from '@/components/Title.vue'
import Inputpage from '@/components/Inputpage.vue'
import Inputpwd from '@/components/Inputpwd.vue'
import Buttonsubmit from '../components/Buttonsubmit.vue'

export default {
  name: 'Login',
  components: {
    Navbar,
    Inputpage,
    Inputpwd,
    Title,
    Buttonsubmit
  }
}
</script>
<style scoped lang="scss">
.home {
  background-image: url("../assets/fondchimievertrose.jpg");

  height: 150vh;
  background-repeat: no-repeat;
  background-size: cover;
}

.content {
  margin-top: 5rem;
}

.text-purple {
  color: #b960ff;
}

.text-green {
  color: #99e48a;
}
</style>