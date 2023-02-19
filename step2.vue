
<template>
  <!--  使用{{}}动态渲染文本-->
  <h1>{{message}}</h1>
  <p>数量是{{counter.count}}</p>
</template>
<script setup>
// 我们可以通过javascript的状态来描述HTML是什么样子的
import { reactive, ref } from 'vue'

// 组件逻辑

// 可以接受任何值，ref会放回一个包裹对象，在.value中使用值
const message = ref('helloo')
// 适用于对象 (包括数组和内置类型，如 Map 和 Set)
const counter = reactive({ count: 0 })
</script>
