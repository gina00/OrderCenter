<template>
<el-scrollbar style="height:100%" wrapClass="scrollbar-wrapper">
    <el-menu default-active="1-1"  class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" background-color="#304156" text-color="#bfcbd9" active-text-color="#409EFF">
        <sidebar-item></sidebar-item>
    </el-menu>
</el-scrollbar>
</template>

<script>
import SiderbarItem from "./SidebarItem";
export default {
    components: {
        "sidebar-item": SiderbarItem
    },
    data() {
        return {
            isCollapse: false
        };
    },
    methods: {
        handleOpen(key, keyPath) {
            console.log(key, keyPath);
        },
        handleClose(key, keyPath) {
            console.log(key, keyPath);
        }
    }
}
</script>

<style lang="scss" scoped>
.el-scrollbar__wrap {
    overflow-y: scroll;
}

.el-menu-vertical-demo:not(.el-menu--collapse) {
    width: 200px;
    min-height: 400px;
}
</style>
