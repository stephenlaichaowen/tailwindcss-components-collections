<template>
  <div class="app">
    <Navigation />
    <div class="content">
      <Card3 />
      <Card2 />
      <Signin />
      <Signup />
    </div>
  </div>
</template>

<script>
import Signin from "./components/Form/Signin.vue";
import Signup from "./components/Form/Signup.vue";
import Alerts from "./components/Alerts.vue";
import Card1 from "./components/Card/Card1.vue";
import Card2 from "./components/Card/Card2.vue";
import Card3 from "./components/Card/Card3.vue";
import Navigation from "./components/Navigation/Navigation.vue";

export default {
  components: {
    Card1,
    Card2,
    Card3,
    Alerts,
    Signin,
    Signup,
    Navigation,
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Quicksand:wght@300;400;500;600;700&family=Roboto:wght@300;400;500;700&display=swap");

/* .app {
  @apply font-sans h-screen flex flex-col justify-center items-center px-8;
} */

.app {
  display: flex;
  flex-direction: column;
  /* height: 100vh; */
  justify-content: center;
}

.content {
  padding: 0 10px;
}

.title {
  @apply text-2xl text-red-500 font-bold;
}
</style>
