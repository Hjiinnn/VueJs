<template>
  <div>
    <input type="text" name="" id="" v-bind:value="userId" readonly />
    <input type="text" name="" id="" :value="userId" readonly />
    <br />
    <img :src="imgSrc" alt="" style="width: 100px; heigth: auto" />
    <br />
    <input type="search" v-model="txt1" />
    <button :disabled="txt1 === ''">조회</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userId: 'jin1234',
      imgSrc: 'https://upload.wikimedia.org/wikipedia/commons/f/f1/Vue.png',
      txt1: ''
    }
  },
  setup() {},
  create() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
