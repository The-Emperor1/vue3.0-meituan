<template>
    <el-header class="header-container">
        <div class="header">
            <i class="icon iconfont icon-dingwei"/>
            <span>{{city}}</span>
            <router-link to='changecity'>切换城市</router-link>
            <div class="near-citys">
                [<a class="city-guess" href="https://lingshan.meituan.com">灵山</a>
                <a class="city-guess" href="https://liaoyang.meituan.com">辽阳</a>
                <a class="city-guess" href="https://haicheng.meituan.com">海城</a>]
            </div>
            <div class='user-entry'>
                <router-link to='sign-in'>立即登录</router-link>
                <router-link to='/'>注册</router-link>
            </div>
            <nav class="nav">
                <ul>
                    <li>我的美团</li>
                    <li>手机APP</li>
                    <li>商家中心</li>
                    <li>美团规则</li>
                    <li>网站导航</li>
                </ul>
            </nav>
        </div>
    </el-header>
</template>

<script>
import { defineComponent, ref } from 'vue'


export default defineComponent({
    setup() {
        const city = ref('上海');
        const onCityChange = () => {
            city.value = '北京';
        }

        return {
            city,
            onCityChange,
        }
    },
})
</script>

<style lang="less" scoped>
    @import url('./index.less');
</style>
