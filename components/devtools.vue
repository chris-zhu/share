<template>
    <h1>devtools 插件</h1>
    <div>
        <NImage src="/devtools001.png" />
    </div>
    <p style="text-align:center;">devtools更好的性能表现</p>
</template>

<script setup lang='ts'>
import { NImage } from 'naive-ui'
</script>
<style lang='scss' scoped>
h1 {
  background-color: #000;
  /* background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%); */
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent; 
  -moz-text-fill-color: transparent;
}
</style>
