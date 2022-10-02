<template>
  <div>
    <div>
      <input
        type="checkbox"
        name=""
        id="html"
        value="html"
        v-model="favoritLang"
      />
      <label for="html">HTML</label>
      <input
        type="checkbox"
        name=""
        id="css"
        value="css"
        v-model="favoritLang"
      />
      <label for="css">CSS</label>
      <input type="checkbox" name="" id="js" value="js" v-model="favoritLang" />
      <label for="js">JS</label>
    </div>
    <div>선택한 언어: {{ favoritLang }}</div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      favoritLang: []
    }
  },
  setup() {},
  create() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
