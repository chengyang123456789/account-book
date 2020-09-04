<template>
<div class="nav-wrapper">
    <div class="content">
        <slot></slot>
    </div>
    <Nav />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Nav from "@/components/Nav.vue";
@Component({
    components:{
        Nav
    }
})
export default class Layout extends Vue {}
</script>
<style lang="scss" scoped>
.nav-wrapper{
    display: flex;
    flex-direction: column;
    border: 1px solid green;
    height: 100vh;
    
}
.content{
    flex-grow: 1;
    overflow: auto;
    
}
</style>