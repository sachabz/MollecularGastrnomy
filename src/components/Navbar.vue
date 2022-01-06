<template>
    <el-menu
        :default-active="activeIndex2"
        class="el-menu-demo"
        mode="horizontal"
        background-color="#000000"
        text-color="#fff"
        active-text-color="#ffd04b"
        @select="handleSelect"
    >
        <el-menu-item>
            <img
                src="../assets/logoMarksblanc.png"
                height="48"
                width="48"
                style="display: inline-block;"
            />
        </el-menu-item>
        <el-menu-item index="1">Processing Center</el-menu-item>
        <el-sub-menu index="2">
            <template #title>Workspace</template>
            <el-menu-item index="2-1">item one</el-menu-item>
            <el-menu-item index="2-2">item two</el-menu-item>
            <el-menu-item index="2-3">item three</el-menu-item>
            <el-sub-menu index="2-4">
                <template #title>item four</template>
                <el-menu-item index="2-4-1">item one</el-menu-item>
                <el-menu-item index="2-4-2">item two</el-menu-item>
                <el-menu-item index="2-4-3">item three</el-menu-item>
            </el-sub-menu>
        </el-sub-menu>
        <el-menu-item index="3" disabled>Info</el-menu-item>
        <el-menu-item index="4">Orders</el-menu-item>
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
</style>