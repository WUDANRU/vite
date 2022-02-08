<template>
  <h1>{{ msg }}</h1>
  <!-- <div>happy new year</div> -->
  <button @click="count++">count is: {{ count }}</button>
  <p>Edit <code>components/HelloWorld.vue</code> to test hot module replacement.</p>
<hr />
<!-- {{count1}} -->
</template>

<script lang="ts">
// import {computed,reactive} from 'vue'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    // const state=reactive({ //这些注释的代码是随便写的，没有效果，主要用于测试打包前后文件大小
    //   count:0
    // })
    return {
      // ...state,
      // count1: computed(()=>state.count*2)
      count: 0
    }
  }
}
</script>
