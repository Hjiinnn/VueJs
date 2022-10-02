<template>
  <div>
    <input type="text" v-model="userId" />
    <p>input tag에서는 v-model="key"를 이용해 양방향 바인딩을 할 수 있다.</p>
    <button @click="myFunction">click!</button>
    <button @click="changeData">Change Data</button>
    <p>클릭 이벤트는 @click="function"을 이용해 바인딩 할 수 있다.</p>
    <br />
    <input type="text" v-model="num1" /> +
    <input type="text" v-model="num2" /> =
    <span>{{ num1 + num2 }}</span>
    <br />
    <input type="text" v-model.number="num3" /> +
    <input type="text" v-model.number="num4" /> =
    <span>{{ num3 + num4 }}</span>
    <p>
      숫자 연산을 위해서는 v-model="key"가 아니라 v-model.number="key"로
      바인딩해주면 된댜.
    </p>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userId: 'write something here!!',
      num1: 0,
      num2: 0,
      num3: 0,
      num4: 0
    }
  },
  setup() {},
  create() {},
  mounted() {},
  unmounted() {},
  methods: {
    myFunction() {
      console.log(this.userId)
    },
    changeData() {
      this.userId = 'change value'
    }
  }
}
</script>
