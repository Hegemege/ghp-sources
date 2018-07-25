<template>
  <div id="app" class="page-full-height flex-container-vertical">
    <Nav></Nav>
    <div class="content flex-item">
        <h1>Test header</h1>
        <p>Test content</p>
    </div>
    <router-view/>
  </div>
</template>

<script>
import { Component, Vue } from "vue-property-decorator";

import Nav from "@/components/Nav";

@Component({
    components: {
        Nav,
    },
})
export default class App extends Vue {}
</script>

<style lang="scss">
@import "@/style.scss";

#nav {
    padding: 30px;
    a {
        font-weight: bold;
        color: #2c3e50;
        &.router-link-exact-active {
            color: #42b983;
        }
    }
}
</style>
