<template>
    <VueUeditorWrap v-model="msg" :config="config"></VueUeditorWrap>
    <p>
        {{ msg }}
    </p>
</template>

<script setup>
import { reactive, ref } from 'vue';
// import VueUeditorWrap from 'vue-ueditor-wrap'
const msg = ref()
const config = reactive({
    UEDITOR_HOME_URL: "/UEditor/",  
    // serverUrl: "/v1/admin/common/uploadTest",  
    // 编辑器不自动被内容撑高  
    autoHeightEnabled: false,  
    // 初始容器高度  
    initialFrameHeight: 500,  
    // 初始容器宽度  
    initialFrameWidth: '100%',  
    lang:'zh-cn'  
})
</script>

<style lang="scss" scoped>

</style>