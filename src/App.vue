<template>
  <div id="app" class="container" >
    <v-story></v-story>
    <v-details></v-details>
    <v-blog-menu></v-blog-menu>
    <v-details-menu></v-details-menu>
  </div>
</template>

<script>
import Story from './components/Story.vue'
import Details from './components/Details.vue'
import BlogMenu from './components/BlogMenu.vue'
import DetailsMenu from './components/DetailsMenu.vue'

export default {
  name: 'app',
  components: {
    VStory: Story,
    VDetails: Details,
    VBlogMenu: BlogMenu,
    VDetailsMenu: DetailsMenu
  }
}
</script>

<style lang="scss">
@import "@/sass/main.scss";
</style>
