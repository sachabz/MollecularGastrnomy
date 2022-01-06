<template>
    <div class="title text-blod">
        <el-button type="success">{{ textbutton }}</el-button>
    </div>
</template>

<script>
export default {
    name: 'Buttonsubmit',
    props: {

        textbutton: String,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.title {
    margin-top: 5rem;
}

.text-bold {
    font-style: bold;
}
</style>
