<template>
  <div>
    <theme-card />
  </div>
</template>

<script>
import themeCard from '@/components/themeCard.vue'

export default {
  components: {
    themeCard
  },
  layout () {
    return 'defaultPage'
  }
}
</script>

<style scoped>

</style>