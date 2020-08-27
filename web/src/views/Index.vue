<template>
    <div id="index">
        <div class="cont">
            <img src="../assets/logo.png" alt="">
            <p class="desc">我的博客</p>
            <div @click="$router.push('/home')" class="btn">进入博客</div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Index'
}
</script>

<style lang="scss">
    html,body{
        width: 100%;
        height: 100%;
    }
    #index{
        width: 100%;
        height: 100%;
        background-image: url('../assets/img/banner.png');
        background-size: 100% 100%;
        background-repeat: no-repeat;
        background-position: center;
        .cont{
            text-align: center;
            padding-top: 200px;
            img{
                width: 84px;
                height: 84px;
                border-radius: 42px;
            }
            p{
                margin: 30px 0;
                color: #fff;
            }
            .btn{
                display: inline-flex;
                align-items: center;
                justify-content: center;
                border-radius: 200px;
                color: #fff;
                border: 1px solid #fff;
                padding: 8px 22px;
                background-color: #24c3ef;
                border-color: #24c3ef;
                cursor: pointer;
            }
        }
    }
</style>