<template>
    <div class="dropdown mt-2">
        <button
            class="btn btn-secondary dropdown-toggle"
            type="button"
            id="dropdownMenu2"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
        >{{ namefilter }}</button>
        <div class="dropdown-menu" aria-labelledby="dropdownMenu2">
            <button class="dropdown-item" type="button">one</button>
            <button class="dropdown-item" type="button">two</button>
            <button class="dropdown-item" type="button">three</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Filter',
    props: {

        namefilter: String,
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.title {
    margin-top: 5rem;
}

.btn {
    background-color: white;
    color: black;
    border-color: #99e48a;
}

.btn:hover {
    color: #99e48a;
}
</style>
