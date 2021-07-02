<template>
    <div>
        <n-space>
            <n-button @click="toggleDark">Is Dark: {{ isDark }}</n-button>
            <n-button @click="showModal = true">组合关系</n-button>
        </n-space>

        <n-modal v-model:show="showModal">
            <n-card  title="组合关系" style="width:1000px;" :bordered="false" size="huge">
                <n-image src="/zuheguanxi.png"></n-image>
            </n-card>
        </n-modal>
    </div>
</template>

<script lang='ts' setup>
import { ref, reactive } from 'vue'
import { NButton, NSpace, NModal, NImage, NCard } from 'naive-ui'
import { useDark, useToggle } from '@vueuse/core'

const isDark = useDark()
const toggleDark = useToggle(isDark)
const showModal = ref(false)
</script>
<style lang='scss' scoped>
</style>
