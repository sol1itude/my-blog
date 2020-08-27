<template>
    <div class="post">
        <mavon-editor
            class="md"
            :value="context"
            :subfield = "prop.subfield"
            :defaultOpen = "prop.defaultOpen"
            :toolbarsFlag = "prop.toolbarsFlag"
            :editable="prop.editable"
            :scrollStyle="prop.scrollStyle"
        ></mavon-editor>
    </div>
</template>

<script>
import md from '../../test.md'

export default {
    name: 'Post',
    data(){
        return {
            context: md,//输入的数据
        }
    },
    mounted() {
        console.log(md);
        this.context = md;
    },
    computed: {
        prop () {
            let data = {
                subfield: false,// 单双栏模式
                defaultOpen: 'preview',//edit： 默认展示编辑区域 ， preview： 默认展示预览区域 
                editable: false,
                toolbarsFlag: false,
                scrollStyle: true
            }
            return data
        }
    },

}
</script>

<style scoped lang="scss">
    .post{
        max-width: 800px;
        margin: 0 auto;
    }
</style>
