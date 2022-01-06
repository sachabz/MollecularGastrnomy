<template>
    <div class="title titlebg">
        <h1 class="font-weight-bold">{{ title }}.</h1>
    </div>
</template>

<script>
export default {
    name: 'Title',
    props: {

        title: String,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.title {
    margin-top: 5rem;
}

.titlebg {
    background-color: rgba(255, 255, 255, 0.397);
}
</style>
