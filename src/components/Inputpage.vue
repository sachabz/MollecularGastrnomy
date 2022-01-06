<template>
    <div class="input py-2 row">
        <div class="col-4"></div>
        <div class="col-2">
            <p class="displaybox">{{ nameinput }}</p>
        </div>
        <div class="col-2">
            <el-input class="displaybox sizebox" v-model="input" clearable />
        </div>
        <div class="col-4"></div>
    </div>
</template>

<script>
export default {
    name: 'Inputpage',
    props: {

        nameinput: String,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
a {
    color: #42b983;
}

.input {
    background-color: rgba(255, 255, 255, 0.397);
}
.displaybox {
    display: inline-block;
}

.sizebox {
    width: 200px;
}
</style>
