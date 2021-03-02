<template>
  <div v-if="isOpen" class="dropdown">
    <a href="/">Docs</a>
    <a href="/">Examples</a>
    <a href="/">Blog</a>
    <button>Download</button>
  </div>
</template>

<script>
export default {
  props: ['isOpen']
};
</script>

<style scoped>
.dropdown {
  background: #14b8a6;
  width: 100vw;
  padding: 12px 0 16px 24px;
  /* display: none; */
}
a {
  color: #99f6e4;
  display: block;
  margin-bottom: 16px;
}
button {
  padding: 8px 16px;
  border-radius: 4px;
  color: white;
  border: 1px solid white;
}
@media (min-width: 575px) {
  .dropdown {
    display: none;
  }
}
</style>
