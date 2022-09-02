<template>
    <VueUeditorWrap v-model="content" :config="config"></VueUeditorWrap>
    <p>
        result:
    </p>
    <p v-html="content">
        
    </p>
</template>

<script setup>
import { reactive, ref } from 'vue';
import { VueUeditorWrap } from 'vue-ueditor-wrap'

const content = ref()

const config = reactive({
    UEDITOR_HOME_URL: "/UEditor/",  
    serverUrl: "//ueditor.zhenghaochuan.com/cos",  
    // 编辑器不自动被内容撑高  
    autoHeightEnabled: false,  
    // 初始容器高度  
    initialFrameHeight: 500,  
    // 初始容器宽度  
    initialFrameWidth: '100%',  
    lang:'zh-cn',
    toolbars:[
        ['kityformula']
    ]
})
</script>

<style lang="scss" scoped>

</style>