<template>
  <div class="col-md-4">
    <div class="position-sticky" style="top: 2rem;">
      <div class="p-4 mb-3 bg-light rounded">
        <h4 class="fst-italic">About</h4>
        <p class="mb-0">Customize this section to tell your visitors a little bit about your publication, writers, content, or something else entirely. Totally up to you.</p>
      </div>

      <div class="p-4">
        <Archives/>
      </div>

      <div class="p-4">
        <h4 class="fst-italic">Follow Me On</h4>
        <ol class="list-unstyled">
          <li><a href="#"><b-icon-github/> GitHub</a></li>
          <li><a href="#"><b-icon-twitter/> Twitter</a></li>
          <li><a href="#"><b-icon-cog/> Facebook</a></li>
        </ol>
      </div>
    </div>
  </div>
</template>

<script>
import Archives from './Archives'
export default {
  name: "Sidebar",
  components:{Archives}
}
</script>

<style scoped>

</style>