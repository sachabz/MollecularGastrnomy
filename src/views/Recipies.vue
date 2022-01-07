<template>
  <div class="home">
    <Navbar />
    <div class="content container">
      <Title title="Recipies" />
      <div class="row">
        <div class="col-lg-3 col-xl-3 col-12 col-sm-3"></div>
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2">
          <Filter namefilter="By category" />
        </div>
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2">
          <Filter namefilter="By date" />
        </div>
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2">
          <Filter namefilter="By difficulty" />
        </div>
        <div class="col-lg-3 col-xl-3 col-12 col-sm-3"></div>
      </div>
      <div class="row contentbg mt-3">
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2"></div>
        <div class="col-lg-4 col-xl-4 col-12 col-sm-4 mt-2 mb-2">
          <img src="../assets/imgrecettes/7.png" class="rounded float-right" />
        </div>
        <div class="col-lg-5 col-xl-5 col-12 col-sm-5">
          <Contentrecipies title="Champignons niamori" time="45min" />
        </div>
        <div class="col-lg-1 col-xl-1 col-12 col-sm-1"></div>
      </div>
      <div class="row contentbg mt-3">
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2"></div>
        <div class="col-lg-4 col-xl-4 col-12 col-sm-4 mt-2 mb-2">
          <img src="../assets/imgrecettes/13.png" class="rounded float-right" />
        </div>
        <div class="col-lg-5 col-xl-5 col-12 col-sm-5">
          <Contentrecipies title="Pola chiken" time="120min" />
        </div>
        <div class="col-lg-1 col-xl-1 col-12 col-sm-1"></div>
      </div>
      <div class="row contentbg mt-3">
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2"></div>
        <div class="col-lg-4 col-xl-4 col-12 col-sm-4 mt-2 mb-2">
          <img src="../assets/imgrecettes/4.png" class="rounded float-right" />
        </div>
        <div class="col-lg-5 col-xl-5 col-12 col-sm-5">
          <Contentrecipies title="Sainte Marina" time="12min" />
        </div>
        <div class="col-lg-1 col-xl-1 col-12 col-sm-1"></div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Navbar from '@/components/Navbar.vue'
import Title from '@/components/Title.vue'
import Filter from '../components/Filter.vue'
import Contentrecipies from '../components/Contentrecipies.vue'


export default {
  name: 'Recipies',
  components: {
    Navbar,
    Title,
    Filter,
    Contentrecipies,

  }
}
</script>
<style scoped lang="scss">
.home {
  background-image: url("../assets/fondchimievertrose4.jpg");

  height: 100vh;
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

img {
  max-width: 100%;
  height: auto;
}

.contentbg {
  background-color: rgba(255, 255, 255, 0.575);
}
</style>