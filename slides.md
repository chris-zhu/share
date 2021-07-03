---
theme: light-icons
layout: image-header-intro
imageHeader: '../assets/images/light-icon-logo.svg'
imageRight: '../assets/images/light-icons-landing.svg'
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
highlighter: shiki
title: Welcome to the sharing session of Chris
---

# 拥抱Vue3

探索前端新的开发体验改善

<!-- <div class="uppercase text-sm tracking-widest">
Chris-zhu
</div> -->

<div class="abs-bl mx-14 my-12 flex">
  <img src="https://2020.vueday.it/img/themes/vueday/vueday-logo.png" class="h-8">
  <div class="ml-3 flex flex-col text-left">
    <div class="uppercase"><b>chris</b>zhu</div>
    <div class="text-sm opacity-50">Jul. 3th, 2021</div>
  </div>
</div>

<img src="http://blog.chrisying.cn/avatar.jpg" class="rounded-full w-40 abs-tr mt-16 mr-12"/>

---

## 一些数据

<div class="body" @click="$slidev.nav.next">
  <div class="left">
    <p><span class="data">1.58M</span> 周活跃用户（devtools插件统计）</p>
    <p><span class="data">9.4M</span> npm 月下载</p>
  </div>
  <div class="right" v-click>
    <p>去年同期对比</p>
    <p>Devtools <span class="data">1.1M -> 1.58M (</span> <span class="numAdd">+43.6%</span> <span>)</span></p>
    <p>NPM <span class="data">6.2M -> 9.4M (</span> <span class="numAdd">+51.6%</span> <span>)</span></p>
  </div>
</div>

<style>
.body{
  width:80%;
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display:flex;
  /* flex-direction: column; */
  justify-content: space-around;
  align-items: center;
}
.data{
  color: #46954A;
}
.numAdd{
  color: #E2B27D;
}
</style>

---

<devtools />

---

# Vue3 生态

<div class="body">
  <!-- vue3 -->
  <div @click="$slidev.nav.next" class="item vue3">
    <img style="width:100px;height:100px;" src="/logo.svg" />
    <span>Vue3</span>
  </div>
  <!-- vite -->
  <div class="item vite" v-click="1">
    <img style="width:100px;height:100px;" src="/vite.svg" />
    <span>Vite@v2</span>
  </div>
  <!-- vue-router@V4 -->
  <div class="item router" v-click="2">
    <img style="width:100px;height:100px;" src="/logo.svg" />
    <span>Vue-Router@v4</span>
  </div>
  <!-- vuex@V4 -->
  <div class="item vuex" v-click="3">
    <img style="width:100px;height:100px;" src="/logo.svg" />
    <span>Vuex@v4</span>
  </div>
  <!-- Typescript -->
  <div class="item js2ts" v-click="4">
    <img style="height:100px;" src="/js2ts.png" />
    <span>Typescript</span>
  </div>
  <!-- UI库 -->
  <div class="item ui" v-click="5">
    <ul>
      <li>
        <img style="width:30px;height:30px;" src="/vant.png" />
        <span>Vant@V3</span>
      </li>
      <li>
        <img style="width:30px;height:30px;" src="/antd.svg" />
        <span>Antd Vue@v2</span>
      </li>
      <li>
        <img style="height:30px;" src="/elementplus.svg" />
      </li>
      <li>
        <img style="width:30px;height:30px;" src="/naive.svg" />
        <span>Naive</span>
      </li>
    </ul>
  </div>
  <!-- utils VueUse -->
  <div class="item vueuse" v-click="6">
    <img style="width:100px;height:100px;" src="/vueuse.svg" />
    <span>VueUse</span>
  </div>
  <!-- Volar -->
  <div class="item volar" v-click="7">
    <img style="width:100px;height:100px;" src="/logo.svg" />
    <span>Volar</span>
  </div>
</div>

<style>
.body{
  width:80%;
  height: 500px;
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display:flex;
  /* flex-direction: column; */
  justify-content: space-around;
  align-items: center;
}
.item{
  display:flex;
  flex-direction: column;
  align-items: center;
}
ul{
  list-style: none;
}
li{
  margin-top:10px;
  display: flex;
}
li span{
  margin-left: 6px;
}
.vite, .router, .vuex, .ui, .volar, .vueuse, .js2ts{
  position: absolute;
}
.vite{
  top: 28px;
  left: 177px;
}
.router{
  top: 153px;
  left: 40px;
}
.vuex{
  top: 312px;
  left: 143px;
}
.vueuse{
  top: 364px;
  left: 337px;
}
.ui{
  top: 309px;
  left: 555px;
}
.js2ts{
  top: 13px;
  left: 393px;
}
.volar{
  top: 94px;
  left: 616px;
}


</style>

---

# Vite 新一代构建工具

<vite />

---

<!-- <volar /> -->

# Type First 类型优先

<div grid="~ cols-2 gap-4">
<div>

开发者体验

- 类型提示
- 智能补全
- 省下写文档的时间
- 方便重构

</div>
<img style="margin-top:100px;" src="/typeFirst001.png"/>
</div>

---

# tsc 的速度不在阻碍开发

<!-- tscbuild.png -->

<div grid="~ cols-2 gap-4">
<div>


- 构建使用esbuild 单纯的typescript 并不会让编译变慢
- 开发时，靠tsserver提示当前文件的类型错误
- CI/CD 时，把tsc作为lint的一部分

</div>
<img style="margin-top:50px;" src="/tscbuild.png"/>
</div>


---

# vscode + volar

更好的IDE支持

编辑器查看

---

# Composition Api (组合式Api)

<p @click="next">什么是组合式Api? 在vue3中引入的一种新的编写Vue组件的方式。</p>

<script setup lang="ts">
import {ref} from 'vue'
const step = ref(0)
const next = ()=>{
  if(step.value >= 5) return
  step.value += 1
}
</script>


<!-- step == 0 -->
<div v-if="step==0" grid="~ cols-2 gap-4">

```ts {all}
<script>
export default {
  data() {
    return {
      dark: false
    }
  },
  computed: {
    light(){
      return !this.dark
    }
  },
  methods: {
    toggle() {
      this.dark = !this.dark
    }
  }
}
</>
```


```ts {all}
<script>
import { ref, computed } from 'vue'
export default {
  setup () {
    const dark = ref(false)
    const light = computed(() => !dark.value)

    return {
      dark,
      light,
      toggle() {
        dark.value = !dark.value
      }
    }
  }
}
</script>
```

</div>

<!-- step == 1 -->
<div v-if="step==1" grid="~ cols-2 gap-4">

```ts {3,7,8,12,13,17}
<script>
export default {
  data() {
    return {
      dark: false
    }
  },
  computed: {
    light(){
      return !this.dark
    }
  },
  methods: {
    toggle() {
      this.dark = !this.dark
    }
  }
}
</script>
```


```ts {4,15}
<script>
import { ref, computed } from 'vue'
export default {
  setup () {
    const dark = ref(false)
    const light = computed(() => !dark.value)

    return {
      dark,
      light,
      toggle() {
        dark.value = !dark.value
      }
    }
  }
}
</script>
```

</div>

<!-- step == 2 -->
<div v-if="step==2" grid="~ cols-2 gap-4">

```ts {4-6}
<script>
export default {
  data() {
    return {
      dark: false
    }
  },
  computed: {
    light(){
      return !this.dark
    }
  },
  methods: {
    toggle() {
      this.dark = !this.dark
    }
  }
}
</script>
```


```ts {5,9}
<script>
import { ref, computed } from 'vue'
export default {
  setup () {
    const dark = ref(false)
    const light = computed(() => !dark.value)

    return {
      dark,
      light,
      toggle() {
        dark.value = !dark.value
      }
    }
  }
}
</script>
```

</div>

<!-- step == 3 -->
<div v-if="step==3" grid="~ cols-2 gap-4">

```ts {8-12}
<script>
export default {
  data() {
    return {
      dark: false
    }
  },
  computed: {
    light(){
      return !this.dark
    }
  },
  methods: {
    toggle() {
      this.dark = !this.dark
    }
  }
}
</script>
```


```ts {6,10}
<script>
import { ref, computed } from 'vue'
export default {
  setup () {
    const dark = ref(false)
    const light = computed(() => !dark.value)

    return {
      dark,
      light,
      toggle() {
        dark.value = !dark.value
      }
    }
  }
}
</script>
```

</div>

<!-- step == 4 -->
<div v-if="step==4" grid="~ cols-2 gap-4">

```ts {13-17}
<script>
export default {
  data() {
    return {
      dark: false
    }
  },
  computed: {
    light(){
      return !this.dark
    }
  },
  methods: {
    toggle() {
      this.dark = !this.dark
    }
  }
}
</script>
```


```ts {11-13}
<script>
import { ref, computed } from 'vue'
export default {
  setup () {
    const dark = ref(false)
    const light = computed(() => !dark.value)

    return {
      dark,
      light,
      toggle() {
        dark.value = !dark.value
      }
    }
  }
}
</script>
```

</div>

<!-- step == 5 -->
<div @click="$slidev.nav.next" v-if="step==5" grid="~ cols-2 gap-4">

```ts {all}
<script>
export default {
  data() {
    return {
      dark: false
    }
  },
  computed: {
    light(){
      return !this.dark
    }
  },
  methods: {
    toggle() {
      this.dark = !this.dark
    }
  }
}
</script>
```


```ts {all}
<script>
import { ref, computed } from 'vue'
export default {
  setup () {
    const dark = ref(false)
    const light = computed(() => !dark.value)

    return {
      dark,
      light,
      toggle() {
        dark.value = !dark.value
      }
    }
  }
}
</script>
```

</div>

---

<whyCompostion v-click="1"/>

<div v-click="2" grid="~ cols-2 gap-4">
  
<div>

对象式API存在的问题

<ul>
  <li v-click="3">不利于复用</li>
  <li v-click="4">潜在的命名冲突</li>
  <li v-click="5">上下文丢失</li>
  <li v-click="6">有限的类型支持</li>
  <li v-click="7">按API类型组织</li>
</ul>

</div>

<div>

组合式API提供的能力

<ul>
  <li v-click="3">极易复用（原生JS函数）</li>
  <li v-click="4">可灵活组合（生命周期钩子可多次使用）</li>
  <li v-click="5">提供更好的上下文支持</li>
  <li v-click="6">更好Typescript类型支持</li>
  <li v-click="7">按功能/逻辑组织</li>
  <li v-click="8">可独立与Vue组件使用</li>
</ul>

</div>

</div>

---

# 什么是组合式函数呢？

我认为它更像是可重用逻辑的集合，使代码更好地组织并分离关注点。

<dark />

```ts {all|2-3|5-15|all}
export function useDark(options: UseDarkOptions = {}) {
  const preferredDark = usePreferredDark()         // <--
  const store = useStorage('vueuse-dark', 'auto')  // <--

  return computed<boolean>({
    get() {
      return store.value === 'auto'
        ? preferredDark.value
        : store.value === 'dark'
    },
    set(v) {
      store.value = v === preferredDark.value 
        ? 'auto' : v ? 'dark' : 'light'
    },
  })
}
```



---

# \<script setup>

<div @click="$slidev.nav.next">

learn at [https://sfc.vuejs.org/](https://sfc.vuejs.org/)


</div>



---

# css in js


<div @click="$slidev.nav.next">

learn at [https://sfc.vuejs.org/](https://sfc.vuejs.org/)


</div>


---
layout: center
class: text-center
---

# 展望未来

Vue未来生态

`Vite` + `Vue3` + `Composition Api` + `Typescript` + `Volar`
