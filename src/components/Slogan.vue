<template>
    <div class="slogan">
        <h1 class="font-weight-bold">
            <slot />
        </h1>
        <h2 class="font-weight-bold">
            <slot name="subtitle" />
        </h2>
        <p>
            <i>{{ auteur }}</i>
        </p>
    </div>
</template>

<script>
export default {
    name: 'Slogan',
    props: {

        auteur: String,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
a {
    color: #42b983;
}

.slogan {
    background-color: rgba(255, 255, 255, 0.397);
}
</style>
