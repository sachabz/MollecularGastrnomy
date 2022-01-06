<template>
    <div class="title">
        <h3 class="font-weight-bold text-left">{{ title }}.</h3>
        <i class="far fa-dot-circle float-left mr-2"></i>
        <i class="far fa-dot-circle float-left mr-2"></i>
        <i class="far fa-dot-circle float-left mr-2"></i>
        <br />
        <p class="text-left">{{ time }}</p>
        <Buttonsubmit textbutton="Cook it" class="mt-1 mb-1 float-left" />
    </div>
</template>

<script>
import Buttonsubmit from './Buttonsubmit.vue'
export default {
    name: 'Contentrecipies',
    components: {
        Buttonsubmit,
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
