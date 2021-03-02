<template>
  <div class="card">
    <div class="image-container">
      <img class="image" src="/coffee.jpeg" alt="woman with coffee" />
    </div>
    <div class="text">
      <div class="label">
        <svg
          class="w-4 h-4"
          fill="currentColor"
          viewBox="0 0 20 20"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
            clip-rule="evenodd"
          ></path>
        </svg>
        <p class="ml-2">Members only</p>
      </div>

      <h4 class="title">Can coffee make you a better developer?</h4>
      <p class="para">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Nihil tempora
        quae repudiandae dignissimos vero nisi soluta optio possimus dolore
        culpa nam nobis sequi amet...
      </p>
      <div class="footer">
        <img class="profile" src="/profile.png" alt="" />
        <div class="content">
          <p class="">Jonathan Reinink</p>
          <p class="date">Aug 18</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.card {
  @apply shadow-xl sm:flex sm:my-16 sm:rounded-tl-md sm:rounded-tr-md;
  max-width: 610px;
  margin: 32px auto;
}
@media (max-width: 640px) {
  .card {
    margin: 0 auto;
  }
}
.image-container {
  @apply sm:w-96;
}
.image {
  @apply w-full h-full sm:rounded-bl-md sm:rounded-tl-md object-cover;  
}
.text {
  @apply p-4;
}
.label {
  @apply text-gray-500 flex items-start align-baseline text-sm;
}
.title {
  @apply font-bold text-2xl mb-1 text-gray-900;
  line-height: 30px;
}
.para {
  @apply font-normal text-gray-700;
}
.footer {
  @apply flex mt-6 items-center;
}
.profile {
  @apply mr-4;
  height: 40px;
}
.content {
  @apply text-gray-600;
}
</style>
