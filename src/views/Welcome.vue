<template>
    <section class="welcome">
      <div id="nav">
        <router-link to="/editor">Create</router-link> |
        <router-link to="/about">About</router-link>
      </div>
      <div class="application-content welcome-content">
        <h1 class="welcome-title">Hi, there!</h1>
        <h2 class="welcome-subtitle"> Make a pretty photo now</h2>
        <Button @click="onClick()">Let's Go!</Button>
      </div>
    </section>
</template>

<script>
import Button from '@/components/Button.vue';

export default {
  name: 'Welcome',
  components: {
    Button,
  },
  methods: {
    onClick() {
      this.$router.push({ name: 'Editor' });
    },
  },
};
</script>

<style lang="scss" scoped>
@import '@/styles/navbar';
.welcome {
  background-color: var(--application-primary-color);
}

.welcome-content{
  display: flex;
  flex-direction: column;
  color: var(--application-text-color);
}

.welcome-title,
.welcome-subtitle {
  margin-bottom: 1.2em;
  text-align: center;
}

.welcome-title{
  margin-top: 8em;
  font-size: 2rem;
  font-weight: 600;
  letter-spacing: 1px;
}

.welcome-subtitle {
  font-size: 1.5rem;
  font-weight: 400;
  letter-spacing: 1px;
}

</style>
