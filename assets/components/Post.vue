<template>
  <article class="blog-post">
    <h2 class="blog-post-title">{{postTitle}}</h2>
    <p class="blog-post-meta">{{publishDate}} by <a href="#">{{author}}</a></p>
    <div v-html="postContent"></div>
  </article>
</template>

<script>
export default {
  name: "Post",
  props:[
      "postTitle",
      "publishDate",
      "author",
      "postContent"
  ]
}
</script>

<style scoped>
/*
 * Blog posts
 */
.blog-post {
  margin-bottom: 4rem;
}
.blog-post-title {
  margin-bottom: .25rem;
  font-size: 2.5rem;
}
.blog-post-meta {
  margin-bottom: 1.25rem;
  color: #727272;
}
</style>