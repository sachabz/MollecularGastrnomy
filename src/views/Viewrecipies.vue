<template>
  <div class="home">
    <div class="content container">
      <router-link to="/Recipies">
        <h1 class="text-green text-right">X</h1>
      </router-link>
      <Title class="m-1" title="Champignons niamori" />
      <Difficulty class="mr-2" />
      <Difficulty class="mr-2" />
      <Difficulty class="mr-2" />
      <p>45min</p>
      <div class="row contentbg mt-3">
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2"></div>
        <div class="col-lg-4 col-xl-4 col-12 col-sm-4 mt-2 mb-2">
          <img src="../assets/imgrecettes/5.png" class="rounded float-right" />
        </div>
        <div class="col-lg-5 col-xl-5 col-12 col-sm-5">
          <Step
            title="Step 1"
            content="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi a. perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi a"
          />
        </div>
        <div class="col-lg-1 col-xl-1 col-12 col-sm-1"></div>
      </div>
      <div class="row contentbg mt-3">
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2"></div>
        <div class="col-lg-4 col-xl-4 col-12 col-sm-4 mt-2 mb-2">
          <img src="../assets/imgrecettes/9.png" class="rounded float-right" />
        </div>
        <div class="col-lg-5 col-xl-5 col-12 col-sm-5">
          <Step
            title="Step 2"
            content="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi a. perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi a"
          />
        </div>
        <div class="col-lg-1 col-xl-1 col-12 col-sm-1"></div>
      </div>
      <div class="row contentbg mt-3">
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2"></div>
        <div class="col-lg-4 col-xl-4 col-12 col-sm-4 mt-2 mb-2">
          <img src="../assets/imgrecettes/12.png" class="rounded float-right" />
        </div>
        <div class="col-lg-5 col-xl-5 col-12 col-sm-5">
          <Step
            title="Step 3"
            content="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi a. perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi a"
          />
        </div>
        <div class="col-lg-1 col-xl-1 col-12 col-sm-1"></div>
      </div>
      <div class="row contentbg mt-3">
        <div class="col-lg-2 col-xl-2 col-12 col-sm-2"></div>
        <div class="col-lg-4 col-xl-4 col-12 col-sm-4 mt-2 mb-2">
          <img src="../assets/imgrecettes/7.png" class="rounded float-right" />
        </div>
        <div class="col-lg-5 col-xl-5 col-12 col-sm-5">
          <Step
            title="Step 4"
            content="Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi a. perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi a"
          />
        </div>
        <div class="col-lg-1 col-xl-1 col-12 col-sm-1"></div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

import Title from '@/components/Title.vue'
import Step from '../components/Step.vue'
import Difficulty from '../components/Difficulty.vue'


export default {
  name: 'Viewrecipies',
  components: {
    Title,
    Step,
    Difficulty

  }
}
</script>
<style scoped lang="scss">
.home {
  background-image: url("../assets/fondchimievertrose4.jpg");

  height: 100vh;
  background-repeat: repeat;
  background-size: cover;
}

.content {
  padding-top: 2rem;
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