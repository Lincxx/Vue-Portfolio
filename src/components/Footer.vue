<template>
  <div class="flex justify-center items-center">
    <div class="h-20 bottom-0 py-8 flex">
      <p class="pr-2">&copy; Jeremy Lincoln</p>
      <a class="github" href="https://github.com/Lincxx/" target="_blank"
        ><GithubCircle
      /></a>
      <a
        class="twitter"
        href="https://twitter.com/MrJeremyLincoln"
        target="_blank"
        ><Twitter
      /></a>
    </div>
    <p>{{ $route.path }}</p>
  </div>
</template>

<script>
import GithubCircle from 'vue-material-design-icons/GithubCircle'
import Twitter from 'vue-material-design-icons/Twitter'
export default {
  name: 'Footer',
  components: {
    GithubCircle,
    Twitter
  }
}
</script>

<style lang="scss" scoped>
.github:hover {
  @apply text-red-700;
}

.twitter:hover {
  @apply text-blue-400;
}
</style>
