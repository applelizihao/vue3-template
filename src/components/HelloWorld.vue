<template>
  <div class="hello">
    <h1>{{ state }}</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent , reactive} from 'vue';

export default defineComponent({
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  setup() {
    const state: object = reactive({
      name:'a'
    })
    return {
      state
    }
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
