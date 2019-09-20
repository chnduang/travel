<template>
  <div class="home-header">
    <div class="header-left">
        <span class="iconfont icon-back">&#xe616;</span>
    </div>
    <div class="header-input">
        <span class="iconfont icon-search">&#xe626;</span>
        <input type="text" placeholder="请输入"/>
    </div>
    <div class="header-right">
        城市
        <span class="iconfont icon-pull">&#xe622;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  components: {},
  data() {
    return {

    }
  }
}
</script>

<style lang="less" scoped>
@import '~styles/global.less';
    .home-header{
        display: flex;
        justify-content: space-between;
        background: @bgColor;
        color: #fff;
        line-height: 3.6rem;
        .header-left{
            width: 3rem;
            text-align: center;
            .icon-back{
                font-size: 1.2rem;
            }
        }
        .header-input{
            flex: 1;
            margin-left: .8rem;
            margin-right: 1rem;
            position: relative;
            .icon-search{
                position: absolute;
                left: .5rem;
                top: .3rem;
                color: #ccc;
            }
            input {
                box-sizing: border-box;
                line-height: 2.4rem;
                width: 100%;
                border-radius: .6rem;
                background: #fff;
                color: #ccc;
                padding-left: 1.8rem;
            }
        }
        .header-right{
            width: 4rem;
            text-align: center;
            .icon-pull{
                font-size: 1rem;
                text-align: center;
            }
        }   
    }

</style>
