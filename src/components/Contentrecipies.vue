<template>
    <div class="title">
        <h3 class="font-weight-bold text-left">{{ title }}.</h3>
        <Difficulty class="float-left mr-2" />
        <Difficulty class="float-left mr-2" />
        <Difficulty class="float-left mr-2" />
        <br />
        <p class="text-left">{{ time }}</p>
        <router-link to="/Viewrecipies">
            <Buttonsubmit textbutton="Cook it" class="mt-1 mb-1 float-left" />
        </router-link>
    </div>
</template>

<script>
import Buttonsubmit from './Buttonsubmit.vue'
import Difficulty from './Difficulty.vue'
export default {
    name: 'Contentrecipies',
    components: {
        Buttonsubmit,
        Difficulty
    },
    props: {

        title: String,
        time: String,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
