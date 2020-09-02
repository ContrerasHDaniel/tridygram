<template>
    <button class="button" @click="onClick()">
        <slot />
    </button>
</template>

<script>
export default {
  name: 'Button',
  methods: {
    onClick() {
      this.$emit('click');
    },
  },
};

</script>

<style lang="scss" scoped>
.button {
    all: unset;
    width: 100%;
    padding: 10px;
    color: var(--application-link-color);
    background-color: var(--application-accent-color);
    border-radius: 5px;
    box-shadow: 0 0 10px 3px rgba(0, 0, 0, 0.1);
    text-transform: uppercase;
    font-weight: 400;
    cursor: pointer;
}

.button:hover {
    color: var(--application-hover-color);
    text-decoration: underline;
    background-color: var(--application-link-color);
}
</style>
