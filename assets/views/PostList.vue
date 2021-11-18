<template>
  <div class="col-md-8">
    <h3 class="pb-4 mb-4 fst-italic border-bottom">
      Recent Posts
    </h3>
    <Post
        post-title="Sample Blog Post"
        publish-date="November 18, 2021"
        author="Caner"
        post-content="<p>Lorem ipsum dolor sit amet.</p><p>Lorem ipsum dolor sit amet.</p><p>Lorem ipsum dolor sit amet.</p>"
    />
    <nav class="blog-pagination" aria-label="Pagination">
      <a class="btn btn-outline-primary" href="#">Older</a>
      <a class="btn btn-outline-secondary disabled">Newer</a>
    </nav>
  </div>
</template>

<script>
import Post from "../components/Post"
export default {
  name: "Content",
  components:{Post}
}
</script>

<style scoped>
/* Pagination */
.blog-pagination {
  margin-bottom: 4rem;
}
.blog-pagination > .btn {
  border-radius: 2rem;
}



</style>