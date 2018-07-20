<template>
  <div id="app" class="page-full-height flex-container-vertical">
    <div id="nav">
      <router-link to="/">Home</router-link>
    </div>
    <div class="content flex-item">
        <h1>Test header</h1>
        <p>Test content</p>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
@import "style.scss";

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
