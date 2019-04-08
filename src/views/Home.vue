<template>
  <div class="home">
    <el-container>
      <el-aside width="220px"><leftList></leftList></el-aside>
      <el-container>
        <el-header height="0">
          <Nav></Nav>
        </el-header>
          <el-main class="a">
            <p class="Statistics">数据统计</p>
            <div class="day-data">
              <el-tag color="orange" size="medium" class="Same-day header">当日数据 :  </el-tag>
              <el-tag color="#e5e9f2" size="medium"  class="Same-day" ><span class="num">7</span>新增用户</el-tag>
              <el-tag color="#e5e9f2" size="medium"  class="Same-day"><span class="num">2</span>新增订单</el-tag>
              <el-tag color="#e5e9f2" size="medium"  class="Same-day"><span class="num">23</span>新增管理员</el-tag>
            </div>
            <div class="total-data">
              <el-tag color="blue" size="medium" class="Same-day header">总数据 :  </el-tag>
              <el-tag color="#e5e9f2" size="medium"  class="Same-day" ><span class="num">23403</span>注册用户</el-tag>
              <el-tag color="#e5e9f2" size="medium"  class="Same-day"><span class="num">8767</span>订单</el-tag>
              <el-tag color="#e5e9f2" size="medium"  class="Same-day"><span class="num">35567</span>管理员</el-tag>
            </div>
          </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import leftList from '@/components/leftList.vue'
import Nav from '@/components/Nav.vue'

export default {
  name: 'home',
  components: {
    HelloWorld,
    leftList,
    Nav
  }
}
</script>


<style lang="less" scoped>
  .home{
    .a{
      background: #fff;
      text-align: left;
      .day-data{
        margin-top: -0.2rem;
      }
      .Statistics{
        text-align: center;
        font-size: .3rem;
        list-style: none;
        font-style: normal;
        height: .4rem;
      }
      .Same-day{
        width: 1.6rem;
        height: .38rem;
        line-height: .38rem;
        text-align: center;
        margin-right: .2rem;
        color: #333;
        border: none;
        margin-top: -2rem;
        .num{
          font-size: .24rem;
          padding-right: .04rem;
        }
      }
      .header{
        color: #fff;
        font-size: .24rem;
        list-style: none;
        font-style: normal
      }
      .total-data{
        height: .3rem;
        margin-top: -1.12rem;
      }
    }
  }
  .el-header, .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }

  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 200px;
  }

  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }
  /*body > .el-container {*/
    /*margin-bottom: 40px;*/
  /*}*/

  el-container:nth-child(5) .el-aside,
  .el-container:nth-child(6) .el-aside {
    line-height: 260px;
  }

  .el-container:nth-child(7) .el-aside {
    line-height: 320px;
  }

</style>
