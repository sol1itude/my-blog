<template>
    <div class="tab d-flex">
        <div @click="curIndex = index" :class="['tab-item', {'active': curIndex === index}]" v-for="(item, index) in tab" :key="index">{{item}}</div>
    </div>
</template>

<script>
export default {
    name: 'Tab',
    data(){
        return {
            curIndex: 0,
            tab: ['首页', '分类', '关于我']
        }
    }
}
</script>

<style scoped lang="scss">
    .tab{
        .tab-item{
            color: #fff;
            padding: 8px 0;
            margin: 0 12px;
            cursor: pointer;
        }
        .active{
            border-bottom: 1px solid #fff;
        }

        
    }
</style>