<template>
    <div  class="right-Nav">
        <span class="size">首页</span>
        <div class="Nav-img">
            <img src="../assets/default.jpg" alt="">
        </div>
    </div>
</template>

<script>

    export default {
        name: "Nav"
    }
</script>

<style scoped lang="less">
    .home{
        position: relative;
        .right-Nav{
            position: absolute;
            top: 0;
            left: 2.18rem;
            z-index: 1000;
            height: .6rem;
            line-height: .6rem;
            width: 84.02%;
            background: #eff2f7;;
            padding-left: .2rem;
            .size{
                position: absolute;
                top: 0;
                left: .2rem;
                font-size: .12rem;
                color: #97a8be;
                cursor: text;
            }
            .Nav-img{
                position: absolute;
                top: .12rem;
                right: .3rem;
                img{
                    width: .36rem;
                    height: .36rem;
                    line-height: .36rem;
                    border-radius: 50%;
                }
            }
        }
    }
</style>