<template>
  <div class="row g-0 border rounded overflow-hidden flex-md-row mb-4 shadow-sm h-md-250 position-relative">
    <div class="col p-4 d-flex flex-column position-static">
      <strong class="d-inline-block mb-2 text-primary">{{postCategory}}</strong>
      <h3 class="mb-0">{{postTitle}}</h3>
      <div class="mb-1 text-muted">{{date}}</div>
      <p class="card-text mb-auto">{{shortText}}</p>
      <a href="#" class="stretched-link">Continue reading</a>
    </div>
    <div class="col-auto d-none d-lg-block">
      <img :src="cardImg">
    </div>
  </div>
</template>

<script>
export default {
  name: "PostCard",
  props:["postTitle","postCategory","date","shortText","cardImg"]
}
</script>

<style scoped>
img{
  width: 200px;
  height: 250px;
}
</style>