<template>
    <vue-ueditor-wrap v-model="msg" :config="config"></vue-ueditor-wrap>

    <p>
        {{ msg }}
    </p>
</template>

<script setup>
import { reactive, ref } from 'vue';
import VueUeditorWrap from 'vue-ueditor-wrap'
const msg = ref()
const config = reactive({
    toolbars:[
        ['']
    ]
})
</script>

<style lang="scss" scoped>

</style>