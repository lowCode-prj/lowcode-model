<template>
    <div class="screen">
            <!-- 引入组件icon1560076112831631360 -->
            <div class="icon1560076112831631360">
                <icon1560076112831631360></icon1560076112831631360>
            </div>
            <!-- 引入组件icon1560076112919711744 -->
            <div class="icon1560076112919711744">
                <icon1560076112919711744></icon1560076112919711744>
            </div>
            <!-- 引入组件icon1560076112936488960 -->
            <div class="icon1560076112936488960">
                <icon1560076112936488960></icon1560076112936488960>
            </div>
    </div>
</template>

<script>
    import Vue from 'vue';
    //引入总线事件以实现大屏组件之间事件的联动
    Vue.prototype.$bus = new Vue();
    // 组件存放的路径 (示例:前端code中vue的相对路径)
    import icon1560076112831631360 from './icon1560076112831631360.vue'

    import icon1560076112919711744 from './icon1560076112919711744.vue'

    import icon1560076112936488960 from './icon1560076112936488960.vue'

    export default {
        components: {
            icon1560076112831631360,
            icon1560076112919711744,
            icon1560076112936488960
        }
    };
</script>

<style lang='less' scoped>
    .screen {
        position: relative;
        width: 1920px;
        height: 1080px;
        background-size: 100% 100%;
        background-color: #232323;
    }
    .icon1560076112831631360{
        height: 100px;
        width: 100px;
        background-color: rgba(34,40,51,0);
        position: absolute;
        top:375px;
        left:679px;
        z-index: 1;
    }
    .icon1560076112919711744{
        height: 100px;
        width: 100px;
        background-color: rgba(34,40,51,0);
        position: absolute;
        top:375px;
        left:868px;
        z-index: 2;
    }
    .icon1560076112936488960{
        height: 100px;
        width: 100px;
        background-color: rgba(34,40,51,0);
        position: absolute;
        top:375px;
        left:1071px;
        z-index: 3;
    }
</style>

