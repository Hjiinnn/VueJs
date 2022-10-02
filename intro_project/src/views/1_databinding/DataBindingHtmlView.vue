<template>
  <div>
    <div>{{ htmlString }}</div>
    <div v-html="htmlString"></div>
    <p>html 바인딩은 v-html="key"로 할 수 있다.</p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      htmlString: '<p style="color:red;">빨간색 문자</p>'
    }
  }
}
</script>
