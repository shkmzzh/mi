<template>
    <div class="nav">
        <div class="container w">
            <ul class="nav-left">
                <li v-for="item in navList" :key="item.id">
                    <a href="#">{{ item.navName }}</a>
                    <div class="sep"></div>
                </li>
            </ul>
            <div class="nav-right">
                <div class="logon">登录</div>
                <div class="sep"></div>
                <div class="register">注册</div>
                <div class="sep"></div>
                <div class="message">消息通知</div>
                <div class="shopping">购物车</div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'App',
    data() {
        return {
            navList: [{ id: 1, navName: '小米官网' }, { id: 2, navName: '小米商城' }, { id: 3, navName: 'MIYUI' }, { id: 4, navName: 'LoT' }, { id: 5, navName: '云服务' }, { id: 6, navName: '天星数科' }, { id: 7, navName: '有品' }, { id: 8, navName: '小爱开放平台' }, { id: 9, navName: '企业团购' }, { id: 10, navName: '资质证照' }, { id: 11, navName: '协议规则' }, { id: 12, navName: '下载app' }, { id: 13, navName: 'Select Location' }]
        }
    },
}
</script>

<style lang="scss" scoped>
.nav {
    height: 40px;
    background-color: #333;
    .container {
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .nav-left {
        display: flex;
        color: #b0b0b0;
        align-items: center;
        height: 100%;
        flex: 1;
        li {
            display: flex;
            align-items: center;

        }

        .sep {
            display: block;
            width: 1px;
            height: 10px;
            background-color: #424242;
            // line-height: 10px;
            margin: 0 10px;
        }
    }

    .nav-right {
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100%;
        color: #b0b0b0;
        font-size: 12px;

        .sep {
            display: block;
            width: 1px;
            height: 10px;
            background-color: #424242;
            // line-height: 10px;
            margin: 0 8px;
        }
        .shopping{
            width: 120px;
            height: 100%;
            background-color: #b0b0b0;
            text-align: center;
            color: red;
            line-height: 40px;
        }
    }
}
</style>
