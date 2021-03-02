<template>
  <div class="card shadow-md">
    <div class="image">
      <img src="/scene.jpg" alt="mountain" />
    </div>
    <div class="content">
      <div class="title">The Coldest Sunset</div>
      <p class="para">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus
        quia, nulla! Maiores et perferendis eaque, exercitationem praesentium
        nihil.
      </p>
      <div class="tags">
        <a href="/">#photography</a>
        <a href="/">#travel</a>
        <a href="/">#winter</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.card {
  max-width: 382px;
  margin: 0 auto 2rem;
  border: 1px solid #eee;
}
.content {
  padding: 16px 24px 16px 24px;
}
.title {
  font-weight: 500;
  font-size: 20px;
  color: #27272a;
  margin-bottom: 8px;
}
.para {
  font-weight: 400;
  line-height: 26px;
  color: #3f3f46;
  margin-bottom: 30px;
}
.tags {
  display: flex;
  flex-wrap: wrap;
}
.tags a {
  background: #F4F4F5;
  padding: 5px 16px;
  margin-right: 11px;
  border-radius: 25px;
  font-size: 12px;
  font-weight: bold;
  color: #3F3F46;
}
</style>
