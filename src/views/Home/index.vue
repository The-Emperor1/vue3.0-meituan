<template>
    <Header />
    <div>首页</div>
</template>

<script>
import './index.less'
import Header from '@/components/Header/index.vue'
import { defineComponent } from 'vue'

export default defineComponent({
    components: {
        Header,
    },
    setup() {
        
    },
})
</script>
