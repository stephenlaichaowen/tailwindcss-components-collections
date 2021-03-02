<template>
  <div class="card">
    <img class="woman" src="/woman.png" alt="" />
    <div class="content">
      <div class="member">
        <img src="/lock.png" alt="lock" />
        <p>Members only</p>
      </div>
      <h4>Can coffee make you a better developer?</h4>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus
        quia, nulla! Maiores et perferendis eaque, exercitationem praesentium
        nihil.
      </p>
      <footer>
        <div class="avatar">
          <img src="/profile.png" alt="avatar" />
        </div>
        <div class="text">
          <p>Jonathan Reinink</p>
          <p>Aug 18</p>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.card {
  display: flex;
  max-width: 610px;
  margin: 2rem auto;
  @apply shadow-xl;
}
@media (max-width: 460px) {
  .card {
    flex-direction: column;
  }
  .card .woman {
    height: 192px;
    @apply object-cover;
  }
}
.content {
  padding: 0 16px;
}
.content h4 {
  font-weight: 700;
  font-size: 20px;
  color: #18181b;
  margin-bottom: 3px;
}
.content p {
  font-weight: 400;
  color: #3f3f46;
}
.member {
  margin-top: 22px;
  display: flex;
  align-items: center;
}
.member img {
  margin-right: 8px;
}
.member p {
  font-size: 14px;
  font-weight: 400;
  color: #52525b;
  line-height: 21px;
}
footer {
  display: flex;
  align-items: center;
  margin-top: 24px;
  margin-bottom: 16px;
}
footer .avatar {
  margin-right: 16px;
}
footer p {
  font-weight: 400;
  color: #3f3f46;
}
</style>
