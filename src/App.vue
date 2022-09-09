<template>
  <div id="app">
    <!-- 跟路由出口 -->
    <router-view/>
  </div>
</template>
<!-- Options API -->
<!--<script lang="ts">
// 1. 编辑器给的类型提示
// 2. TypeScript 编译期间的类型验证

import Vue from 'vue'
export default Vue.extend({
  data () {
    return {
      a: 1,
      b: '2',
      c: [],
      d: {
        a: 1,
        b: '2'
      }
    }
  }
})
</script>-->

<!-- ClassAPI -->
<!-- <script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'

@Component // 调用类的装饰器
export default class App extends Vue {
  a = 1
  b = '2'
  c = {
    a: 1,
    b: '2'
  }

  test () {
    console.log(this.a)
    // this.b
    // this.a.abc()
  }

  created () {
    console.log('app created')
  }
}
</script>-->
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'App'
})
</script>

<style lang="scss" scoped></style>
