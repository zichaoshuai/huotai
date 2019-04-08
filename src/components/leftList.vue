<template>
    <div id="app">
        <el-row class="tac">
            <el-col>
                <el-menu
                        default-active="2"
                        class="el-menu-vertical-demo"
                        @open="handleOpen"
                        @close="handleClose">
                    <el-menu-item index="7" class="line">
                        <i class="el-icon-menu ele" ></i>
                        <span slot="title">首页</span>
                    </el-menu-item>
                    <el-submenu index="1" class="line">
                        <template slot="title">
                            <i class="iconfont icon-zhizhang3"></i>
                            <span class="data">数据管理</span>
                        </template>
                        <el-menu-item-group>
                            <el-menu-item index="1-1"><a href="/userList">用户列表</a></el-menu-item>
                            <el-menu-item index="1-2">商家列表</el-menu-item>
                            <el-menu-item index="1-3">食品列表</el-menu-item>
                            <el-menu-item index="1-4">订单列表</el-menu-item>
                            <el-menu-item index="1-5">管理员列表</el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>
                    <el-submenu index="2" class="line">
                        <template slot="title">
                            <i class="el-icon-plus ele"></i>
                            <span class="data">添加数据</span>
                        </template>
                        <el-menu-item-group>
                            <el-menu-item index="2-1">添加商铺</el-menu-item>
                            <el-menu-item index="2-2">添加商品</el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>
                    <el-submenu index="3" class="line">
                        <template slot="title">
                            <i class="el-icon-star-on ele"></i>
                            <span>图表</span>
                        </template>
                        <el-menu-item-group>
                            <el-menu-item index="3-1">用户分布</el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>
                    <el-submenu index="4" class="line">
                        <template slot="title">
                            <i class="iconfont icon-bi"></i>
                            <span>编辑</span>
                        </template>
                        <el-menu-item-group>
                            <el-menu-item index="4-1">文本编辑</el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>
                    <el-submenu index="5" class="line">
                        <template slot="title">
                            <i class="iconfont icon-settings"></i>
                            <span>设置</span>
                        </template>
                        <el-menu-item-group>
                            <el-menu-item index="5-1">管理员设置</el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>
                    <el-submenu index="6" class="line">
                        <template slot="title">
                            <i class="iconfont icon-shuoming"></i>
                            <span>说明</span>
                        </template>
                        <el-menu-item-group>
                            <el-menu-item index="6-1">说明</el-menu-item>
                        </el-menu-item-group>
                    </el-submenu>
                </el-menu>
            </el-col>
        </el-row>
    </div>

</template>

<script>
    export default {
        methods: {
            handleOpen(key, keyPath) {
                // console.log(key, keyPath);
            },
            handleClose(key, keyPath) {
                // console.log(key, keyPath);
            }
        }
    }
</script>

<style scoped lang="less">
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        .tac{
            .line{
                position: relative;
                .iconfont {
                    position: absolute;
                    left: .22rem;
                }
                .ele{
                    position: absolute;
                    left: .19rem;
                    top: .19rem;
                }
                span{
                    padding-right: .8rem;
                }
                .data{
                    margin-left: .24rem;
                }
            }

        }
    }
    #nav {
        padding: .3rem;
        a {
            font-weight: bold;
            color: #2c3e50;
            &.router-link-exact-active {
                color: #42b983;
            }
        }
    }
</style>