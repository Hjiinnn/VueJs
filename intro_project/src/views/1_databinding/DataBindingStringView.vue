<template>
  <div>
    <h1>Hello {{ userName }}.</h1>
    <p>문자열 데이터 바인딩은 {{ message }} 중괄호 2개로 묶어준다.</p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      userName: 'John Doe',
      message: '{{}}'
    }
  }
}
</script>
<style scoped>
.text-red {
  color: red;
}
</style>
