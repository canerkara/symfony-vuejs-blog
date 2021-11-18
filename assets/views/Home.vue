<template>
<div>
  <b-container>
    <div class="p-4 p-md-5 mb-4 text-white rounded bg-dark">
      <div class="col-md-6 px-0">
        <h1 class="display-4 fst-italic">Title of a longer featured blog post</h1>
        <p class="lead my-3">Multiple lines of text that form the lede, informing new readers quickly and efficiently about what’s most interesting in this post’s contents.</p>
        <p class="lead mb-0"><a href="#" class="text-white fw-bold">Continue reading...</a></p>
      </div>
    </div>
    <div class="row mb-2">
      <div class="col-md-6">
        <PostCard
            post-title="Post Title"
            card-img="https://via.placeholder.com/200x250.png?text=Thumbnail"
            date="Nov 18"
            post-category="World"
            short-text="Lorem ipsum dolor sit amet."
        />
      </div>
      <div class="col-md-6">
        <PostCard
            post-title="Post Title"
            card-img="https://via.placeholder.com/200x250.png?text=Thumbnail"
            date="Nov 18"
            post-category="World"
            short-text="Lorem ipsum dolor sit amet."
        />
      </div>
    </div>
    <div class="row g-5">
      <PostList/>
      <Sidebar/>
    </div>

  </b-container>


</div>
</template>

<script>
import Sidebar from "../components/Sidebar"
import PostCard from "../components/PostCard"
import PostList from "../views/PostList"
export default {
  name: "Home",
  components: {PostList, PostCard, Sidebar}
}
</script>

<style scoped>
.card-img-right {
  height: 100%;
  border-radius: 0 3px 3px 0;
}
</style>