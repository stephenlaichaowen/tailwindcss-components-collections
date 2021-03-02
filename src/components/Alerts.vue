<template>
  <div class="alerts">
    <div class="type1">
      <p><b class="text-red-700 font-bold">Holy smokes!</b> Something seriously bad happened.</p>
      <div class="close">
        <svg
          class="w-5 h-5 text-red-500"
          fill="currentColor"
          viewBox="0 0 20 20"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
            clip-rule="evenodd"
          ></path>
        </svg>
      </div>
    </div>
    <div class="type2"></div>
    <div class="type3"></div>
    <div class="type4"></div>
    <div class="type5"></div>
    <div class="type6"></div>
    <div class="type7"></div>
  </div>
</template>

<style scoped>
.type1 {
  @apply flex items-center py-2.5 pl-4 pr-2.5 rounded-md border border-red-600;
  background: #fee2e2;    
}
.type1 p {
  @apply text-red-600 mr-12;
}
</style>
