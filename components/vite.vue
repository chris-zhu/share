<template>
  <div class="body">
    <div class="left">
      <div class="vite">
        <img @click="num += 1" src="/vite.svg" alt />
        <p>
          learn more at
          <n-a href="https://cn.vitejs.dev/" target="_blank">https://cn.vitejs.dev</n-a>
        </p>
      </div>
    </div>
    <div class="right">
      <n-ul align-text>
        <n-li v-if="num >= 1">类似vue-cli的熟悉体验</n-li>
        <n-li v-if="num >= 2">基于原生ESM的极速热更新</n-li>
        <n-li v-if="num >= 3">基于esbuild的依赖预打包</n-li>
        <n-li v-if="num >= 4">兼容rollup的插件机制</n-li>
        <n-li v-if="num >= 5">内置SSR支持</n-li>
        <n-li @click="$slidev.nav.next" v-if="num >= 6">...</n-li>
      </n-ul>
    </div>
  </div>
</template>

<script lang='ts' setup>
import { ref } from 'vue'
import {NUl, NLi, NA} from 'naive-ui'
const num = ref(0)
</script>

<style lang="scss" scoped>
.body {
  display: flex;
  justify-content: center;
}
.vite {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
img {
  width: 150px;
}
.right{
  margin-left:100px;
  width:400px;
}
</style>
