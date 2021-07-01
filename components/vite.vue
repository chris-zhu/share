<template>
  <div class="body">
    <div class="left">
      <div class="vite">
        <img @click="num++" src="/vite.svg" alt="vite"/>
        <p>
          <span @click="num--">learn more at </span> 
          <n-a href="https://cn.vitejs.dev/" target="_blank">https://cn.vitejs.dev</n-a>
        </p>
      </div>
    </div>
    <div class="right">
      <div v-if="showPics">
        <n-image-group>
          <n-space>
            <n-image
              width="500"
              src="/viteWebpack001.png"
            />
            <n-image
              width="500"
              src="/viteWebpack002.png"
            />
          </n-space>
        </n-image-group>
      </div>
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
import { ref,computed } from 'vue'
import {NUl, NLi, NA, NImage, NImageGroup, NSpace} from 'naive-ui'
const num = ref(0)
const showPics = computed(() => {
  return num.value <= 0
})
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
