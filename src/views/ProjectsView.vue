<script>
  import GithubProjects from '../components/GithubProjects.vue';

  export default {
  components: {
    GithubProjects, // Register the component
  },
};
</script>

<template>
  <div class="projects">
    <GithubProjects></GithubProjects>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
