<template>
<section class="app-main">
    <transition  name="fade-transform" mode="out-in" appear='true'>
        <router-view></router-view>
    <div>maincontent</div>
    </transition>
</section>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>

</style>

