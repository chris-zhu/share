---
theme: light-icons
# layout: intro
layout: image-header-intro
imageHeader: '../assets/images/light-icon-logo.svg'
imageRight: '../assets/images/light-icons-landing.svg'
image: 'https://source.unsplash.com/collection/94734566/1920x1080'
class: text-center
highlighter: shiki
title: Welcome to the sharing session of Chris
---

# 拥抱

探索前端新的开发体验改善

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 p-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<!-- <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
  class="abs-br m-6 text-xl icon-btn opacity-50 !border-none !hover:text-white">
  <carbon-logo-github />
</a> -- >

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)asd
-->

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

# devtools 插件

<div @click="$slidev.nav.next">
  <img src="/devtools001.png"/>
</div>

<p style="text-align:center">devtools 更好的性能表现</p>

<style>
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

# Vite

<vite />

---

<!-- <volar /> -->

# Type First 类型优先

<div grid="~ cols-2 gap-4">
<div>

- 类型提示
- 智能补全
- 省下写文档的时间
- 方便重构

</div>
<div>
  示例代码



</div>
</div>



---

# Navigation

Hover on the bottom-left corner to see the navigation's controls panel, [learn more](https://sli.dev/guide/navigation.html)

### Keyboard Shortcuts

|                                     |                             |
| ----------------------------------- | --------------------------- |
| <kbd>right</kbd> / <kbd>space</kbd> | next animation or slide     |
| <kbd>left</kbd>                     | previous animation or slide |
| <kbd>up</kbd>                       | previous slide              |
| <kbd>down</kbd>                     | next slide                  |

<!-- https://sli.dev/guide/animations.html#click-animations -->

<img
  v-click
  class="absolute -bottom-9 -left-7 w-80 opacity-50"
  src="https://sli.dev/assets/arrow-bottom-left.svg"
/>

<p v-after class="absolute bottom-23 left-45 opacity-30 transform -rotate-10">Here!</p>
<h1>123</h1>

---

# Code

Use code snippets and get the highlighting directly!

<!-- https://sli.dev/guide/syntax.html#line-highlighting -->

```ts {monaco}
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: User) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

<arrow v-click="3" x1="400" y1="420" x2="230" y2="330" color="red" width="3" arrowSize="1" />

---

# Components

<div grid="~ cols-2 gap-4">
  <div>

You can use Vue components directly inside your slides.

We have provided a few built-in components like `<Tweet/>` and `<Youtube/>` that you can use directly. And adding your custom components is also super easy.

```html
<Counter :count="10" />
```

  <!-- ./components/Counter.vue -->
  <Counter :count="10" m="t-4" />

Check out [the guides](https://sli.dev/builtin/components.html) for more.

  </div>
  <div>

```html
<Tweet id="1390115482657726468" />
```

  <Tweet id="1390115482657726468" scale="0.65" />

  </div>
</div>

---

## class: px-20

# Themes

Slidev comes with powerful theming support. Themes can provide styles, layouts, components, or even configurations for tools. Switching between themes by just **one edit** in your frontmatter:

<div grid="~ cols-2 gap-2" m="-t-2">

```yaml
---
theme: default
---
```

```yaml
---
theme: seriph
---
```

<img border="rounded" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-default/01.png?raw=true">

<img border="rounded" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-seriph/01.png?raw=true">

</div>

Read more about [How to use a theme](https://sli.dev/themes/use.html) and
check out the [Awesome Themes Gallery](https://sli.dev/themes/gallery.html).

---

## preload: false

# Animations

Animations are powered by [@vueuse/motion](https://motion.vueuse.org/).

```html
<div v-motion :initial="{ x: -80 }" :enter="{ x: 0 }">Slidev</div>
```

<div class="w-60 relative mt-6">
  <div class="relative w-40 h-40">
    <img
      v-motion
      :initial="{ x: 800, y: -100, scale: 1.5, rotate: -50 }"
      :enter="final"
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-square.png"
    />
    <img
      v-motion
      :initial="{ y: 500, x: -100, scale: 2 }"
      :enter="final"
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-circle.png"
    />
    <img
      v-motion
      :initial="{ x: 600, y: 400, scale: 2, rotate: 100 }"
      :enter="final"
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-triangle.png"
    />
  </div>

  <div 
    class="text-5xl absolute top-14 left-40 text-[#2B90B6] -z-1"
    v-motion
    :initial="{ x: -80, opacity: 0}"
    :enter="{ x: 0, opacity: 1, transition: { delay: 2000, duration: 1000 } }">
    Slidev
  </div>
</div>

<!-- vue script setup scripts can be directly used in markdown, and will only affects current page -->
<script setup lang="ts">
const final = {
  x: 0,
  y: 0,
  rotate: 0,
  scale: 1,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
</script>

<div
  v-motion
  :initial="{ x:35, y: 40, opacity: 0}"
  :enter="{ y: 0, opacity: 1, transition: { delay: 3500 } }">

[Learn More](https://sli.dev/guide/animations.html#motion)

</div>

---

# LaTeX

LaTeX is supported out-of-box powered by [KaTeX](https://katex.org/).

<br>

Inline $\sqrt{3x-1}+(1+x)^2$

Block

$$
\begin{array}{c}

\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} &
= \frac{4\pi}{c}\vec{\mathbf{j}}    \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\

\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\

\nabla \cdot \vec{\mathbf{B}} & = 0

\end{array}
$$

<br>

[Learn more](https://sli.dev/guide/syntax#latex)

---

# Diagrams

You can create diagrams / graphs from textual descriptions, directly in your Markdown.

<div class="grid grid-cols-2 gap-4 pt-4 -mb-6">

```mermaid {scale: 0.9}
sequenceDiagram
    Alice->John: Hello John, how are you?
    Note over Alice,John: A typical interaction
```

```mermaid {theme: 'neutral', scale: 0.8}
graph TD
B[Text] --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```

</div>

[Learn More](https://sli.dev/guide/syntax.html#diagrams)

---

layout: center
class: text-center

---

# Learn More

[Documentations](https://sli.dev) / [GitHub Repo](https://github.com/slidevjs/slidev)
