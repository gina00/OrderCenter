<template>
<div>
    <div class="side-content">
        <side-bar></side-bar>
    </div>
    <div class="main-content">
        <nav-bar></nav-bar>
        <app-main></app-main>
    </div>
</div>
</template>

<script>
import SideBar from './components/Sidebar/index'
import AppMain from './components/AppMain'
import NavBar from './components/NavBar'
export default {
    components:{
        'side-bar':SideBar,
        'nav-bar':NavBar,
        'app-main':AppMain
    }

}
</script>

<style lang="scss" scoped>

.main-content{
    min-height: 100%;
    -webkit-transition: margin-left .28s;
    transition: margin-left .28s;
    margin-left: 180px;
    position: relative;
}
</style>
