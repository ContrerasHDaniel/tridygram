<template>
  <section>
    <div id="app">
      <router-view class="application-container"/>
    </div>
  </section>
</template>

<style lang="scss">
@import '@/styles/reset';
@import '@/styles/layout';

body{
  margin: 0;
  height: 0;

  // CSS Variables
  //Colors
  --application-primary-color: #F6BD60;
  --application-text-color: #5D576B;
  --application-accent-color: #141301;
  --application-link-color: #ED6A5A;
  --application-hover-color: #F7F5FB;
}

* {
  box-sizing: border-box;
}

#app {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Aria
                sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
