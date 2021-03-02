<template>
  <Navbar @toggle="toggle" />
  <Dropdown :isOpen="isOpen" />
</template>

<script>
import Navbar from './Navbar.vue'
import Dropdown from './Dropdown.vue'
import { ref } from 'vue'

export default {
  components: {
    Navbar,
    Dropdown
  },
  setup() {
    const isOpen = ref(false)
    
    const toggle = () => {
      isOpen.value = !isOpen.value
    }

    return { isOpen, toggle }
  }
};
</script>

<style scoped></style>
