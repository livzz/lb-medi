<template>
  <div>
    <p class="text-lg" v-if="!large && !semiLarge">{{text}}</p>
    <p class="text-2xl" v-else-if="semiLarge">{{text}}</p>
    <p class="text-2xl" v-else>{{text}}</p>
  </div>
</template>

<script>
export default {
  props: {
    text: String,
    large: Boolean,
    semiLarge: Boolean
  }
}
</script>

<style scoped>
</style>