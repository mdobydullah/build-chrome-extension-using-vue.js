<template>
  <div class="extension">
    <h2>Search on MyNotePapar</h2>

    <input v-model="keyword" placeholder="Enter keyword">
    <button v-on:click="buttonSearch">Search</button>

    <p>To get more articles visit <a target="_blank" href="https://www.mynotepaper.com/" style="text-decoration: none;">mynotepaper.com</a></p>
  </div>
</template>

<script>
const browser = require("webextension-polyfill");
export default {
  data() {
    return {
      keyword: "",
    };
  },
  methods: {
    buttonSearch() {
      	window.open("https://www.mynotepaper.com/?s=" + this.keyword);
    }
  }
};
</script>

<style lang="scss" scoped>
p {
  font-size: 16px;
}
.extension {
  width: 300px;
  text-align: center;
}
</style>