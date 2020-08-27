<template>
    <div class="header">
        <div class="head d-flex jc-space-between al-center">
            <img src="@/assets/logo.png" alt="">
            <Tab />
        </div>
    </div>
</template>

<script>
import Tab from './Tab'
export default {
    name: 'Header',
    components: {
        Tab
    }
}
</script>

<style scoped lang="scss">
    .header{
        width: 100%;
        height: 80px;
        background-color: #000;
        position: sticky;
        top: 0;
        z-index: 99;
        .head{
            width: 1200px;
            min-width: 1200px;
            height: 100%;
            margin: 0 auto;
            img{
                width: 40px;
                height: 40px;
                border-radius: 20px;
            }
        }
    }
</style>