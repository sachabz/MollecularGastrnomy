<template>
    <div class="slogan">
        <h1 class="font-weight-bold">{{ msg }}</h1>
        <h1 class="font-weight-bold">{{ msg2 }}</h1>
        <p>{{ auteur }}</p>
    </div>
</template>

<script>
export default {
    name: 'Slogan',
    props: {
        msg: String,
        msg2: String,
        auteur: String,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Rokkitt:wght@400;800&display=swap");
h1 {
    font-family: "Rokkitt", serif;
}
ul {
    list-style-type: none;
    padding: 0;
}
li {
    display: inline-block;
    margin: 0 10px;
}
a {
    color: #42b983;
}

.slogan {
    background-color: rgba(255, 255, 255, 0.397);
}
</style>
