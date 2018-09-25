<template>
<div>

<el-menu-item index="1">
        <i class="el-icon-menu"></i>
        <span slot="title">概览</span>
    </el-menu-item>

    <el-submenu index="2">
        <template slot="title">
            <i class="el-icon-location"></i>
            <span>导航一</span>
        </template>
        <el-menu-item-group>
            <el-menu-item index="1-1">选项1</el-menu-item>
            <el-menu-item index="1-2">选项2</el-menu-item>
            <el-menu-item index="1-3">选项3</el-menu-item>
        </el-menu-item-group>
        <el-submenu index="1-4">
            <template slot="title">选项4</template>
            <el-menu-item index="1-4-1">选项1</el-menu-item>
        </el-submenu>
    </el-submenu>
    <el-menu-item index="3">
        <i class="el-icon-menu"></i>
        <span slot="title">导航二</span>
    </el-menu-item>
    <el-menu-item index="4">
        <i class="el-icon-setting"></i>
        <span slot="title">导航四</span>
    </el-menu-item>
    <el-menu-item index="5">
        <span slot="title">状态值：{{$store.state.app.count}}</span>
    </el-menu-item>
</div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.el-menu-item-group{
    ul{
        background: #333;
    }
}
</style>
