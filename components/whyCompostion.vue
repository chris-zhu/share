<template>
  <h1 @click="show = !show">为什么要引入组合式Api</h1>
  <div class="body" v-if="show" >
    <n-image src="/optionApi.jpeg" width="150" />
    <n-image src="/compositionApi.jpg" width="150" />
  </div>
</template>

<script lang='ts' setup>
import { NImage } from 'naive-ui'
import { ref } from 'vue'
const show = ref(true)
</script>
<style lang='scss' scoped>
.body {
  display: flex;
  justify-content: space-around;
}
</style>
