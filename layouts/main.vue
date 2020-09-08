<template>
  <div>
    <headerBlock />
    <div class="center">
      <Nuxt />
    </div>
  </div>
</template>

<script>
import headerBlock from '../components/headerBlock.vue'

export default {
  head() {
    return {
      link: [
        { rel: 'canonical', href: `http://localhost:3000${this.$route.path}` },
      ],
    }
  },
  components: {
    headerBlock,
  },
}
</script>

<style></style>
