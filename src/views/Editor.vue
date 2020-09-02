<template>
  <section class="editor">
    <div id='nav'>
      <router-link to="/">Welcome</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <div id='sidenav'>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Editor',
};
</script>

<style lang="scss" scoped>
@import '@/styles/navbar';

.editor {
  background-color: var(--application-primary-color);
}

#sidenav{
  width: 15%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
</style>
