<template>
    <div class="content">
        <div class="article-list">
            <div class="article-item" v-for="(articleItem, index) in articleList" :key="index">
                <div class="title">{{articleItem.title}}</div>
                <div class="d-flex al-center">
                    <p>{{articleItem.author}}</p><p> | </p><p>{{articleItem.date}}</p>
                </div>
                <div class="cover">
                    <img :src="articleItem.cover" alt="">
                </div>
                <div class="descript">{{articleItem.descript}}</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Content',
    data() {
        return {
            articleList: [
                {
                    title: '前端学习路程',
                    author: 'misswang',
                    date: '2020-08/-27 18:06',
                    cover: require('../assets/img/banner.png'),
                    descript: '这段时间莫名的对ssr产生了兴趣，开始捣鼓着把原来用`create-react-app`的项目用`next.js`重构成服务端渲染。下面记录一下一些要点以及踩坑之旅'
                },{
                    title: '前端学习路程',
                    author: 'misswang',
                    date: '2020-08/-27 18:06',
                    cover: require('../assets/img/banner.png'),
                    descript: '这段时间莫名的对ssr产生了兴趣，开始捣鼓着把原来用`create-react-app`的项目用`next.js`重构成服务端渲染。下面记录一下一些要点以及踩坑之旅'
                },{
                    title: '前端学习路程',
                    author: 'misswang',
                    date: '2020-08/-27 18:06',
                    cover: require('../assets/img/banner.png'),
                    descript: '这段时间莫名的对ssr产生了兴趣，开始捣鼓着把原来用`create-react-app`的项目用`next.js`重构成服务端渲染。下面记录一下一些要点以及踩坑之旅'
                },{
                    title: '前端学习路程',
                    author: 'misswang',
                    date: '2020-08/-27 18:06',
                    cover: require('../assets/img/banner.png'),
                    descript: '这段时间莫名的对ssr产生了兴趣，开始捣鼓着把原来用`create-react-app`的项目用`next.js`重构成服务端渲染。下面记录一下一些要点以及踩坑之旅'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .content{
        width: 980px;
        min-width: 980px;
        margin: 0 auto;
        .article-list{
            .article-item{
                padding: 30px 0;
                border-bottom: 1px solid #ededed;
                .title{
                    margin-bottom: 20px;
                    font-size: 24px;
                }
                .d-flex{
                    color: #969696
                }
                .cover{
                    margin: 20px 0;
                    img{
                        width: 100%;
                    }
                }
                .descript{
                    line-height: 1.5;
                }
            }
        }
    }
</style>