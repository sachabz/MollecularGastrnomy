<template>
    <div class="title">
        <h3 class="font-weight-bold text-left">{{ title }}</h3>
        <p class="text-left">{{ content }}</p>
    </div>
</template>

<script>

export default {
    name: 'Step',
    components: {

    },
    props: {

        title: String,
        content: String,

    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
</style>
