<template>
  <div class="nav">
    <router-link to="/money">记账</router-link>|
    <router-link to="/labels">标签</router-link>|
    <router-link to="/statistics">统计</router-link>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import x from "@/assets/icons/label.svg";
@Component
export default class Nav extends Vue {
  created() {
    console.log(x);
  }
}
</script>

<style lang="scss" scoped>
.nav {
  border: 1px solid red;
}
</style>