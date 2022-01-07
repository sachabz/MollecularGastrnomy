<template>
    <el-menu
        :default-active="activeIndex2"
        class="el-menu-demo px-4"
        mode="horizontal"
        background-color="#000000"
        text-color="#fff"
        active-text-color="#99E48A"
        @select="handleSelect"
    >
        <el-menu-item>
            <router-link to="/">
                <span>
                    <img
                        src="../assets/logoMarksblanc.png"
                        height="48"
                        width="48"
                        style="display: inline-block; vertical-align: middle"
                    />
                </span>
            </router-link>
            <el-menu-item index="1">
                <router-link to="/recipies">Recipies.</router-link>
            </el-menu-item>
            <form class="form-inline my-2 my-lg-0">
                <input
                    class="form-control mr-sm-2"
                    type="search"
                    placeholder="Search"
                    aria-label="Search"
                />
                <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
            </form>
        </el-menu-item>
        <el-menu-item index="2">
            <router-link to="/login">Login|Register.</router-link>
        </el-menu-item>
        <el-menu-item index="3">
            <span>
                <i class="far fa-user" style="display: inline-block; vertical-align: middle"></i>
            </span>
        </el-menu-item>
    </el-menu>
</template>

<script>

export default {
    name: 'Navbar',
    props: {

    }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.navbar {
    width: 100vw;
}
.btn {
    color: #99e48a;
    border-color: #99e48a;
    font-size: 14px;
}

.form-control {
    font-size: 14px;
}
.btn:hover {
    background-color: #99e48a;
    color: white;
}

.fa-user:hover {
    color: #99e48a;
}
</style>