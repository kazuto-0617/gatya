<template>
  <div class="home">
    <h1>ガチャ</h1>
    <div v-if="resultShow">
      <p>{{ item1 }}</p>
      <p>{{ item2 }}</p>
      <p>{{ item3 }}</p>
    </div>
    <button @click="turnTheGatya">回す</button>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  components: {},
  data() {
    return {
      item1: "商品1",
      item2: "商品2",
      item3: "商品3",
      resultShow: false,
    };
  },
  methods: {
    turnTheGatya() {
      this.item1 = "商品5";
      this.resultShow = true;
    },
  },
};
</script>
