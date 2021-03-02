<template>
  <div class="navbar">
    <div class="logo">
      <div class="logo-img">
        <img src="/logo.png" alt="" />
      </div>
      <p>Tailwind CSS</p>
    </div>
    <div class="menu">
      <a href="/">Docs</a>
      <a href="/">Examples</a>
      <a href="/">Blog </a>
    </div>
    <button>Download</button>
    <div class="burger" @click="toggle">
      <img src="/burger.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
  // setup({ emit }) {

  //   const toggle = () => emit('toggle')

  //   return { toggle }
  // }
  methods: {
    toggle() {
      this.$emit('toggle')
    }
  },
};
</script>

<style scoped>
.navbar {
  /* max-width: 100vw; */
  padding: 20px 36px 20px 24px;
  background: #14b8a6;
  display: flex;
  align-items: center;
}
.logo {
  display: flex;
  align-items: center;
}
.logo-img {
  width: 32px;
  height: 32px;
  display: flex;
  align-items: center;
  margin-right: 8px;
}
.logo p {
  font-size: 20px;
  font-weight: 700;
  color: white;
  margin-right: 30px;
}
a {
  color: #99F6E4;
  margin-right: 24px;
  font-weight: 400;  
}
button {
  margin-left: auto;
  padding: 8px 16px;
  border-radius: 4px;
  color: white;
  border: 1px solid white;
}
.burger {
  margin-left: auto;
  display: none;
}
@media (max-width: 575px) {
  button {
    display: none;
  }
  .menu {
    display: none;
  }
  .burger {
    display: block;
  }
}
</style>
