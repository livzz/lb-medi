<template>
  <div>
    <h3 class="xl:text-3xl lg:text-2xl" :class="extraClass" v-if="!large">{{text}}</h3>
    <h3 class="xl:text-4xl lg:text-2xl" :class="extraClass" v-else>{{text}}</h3>
  </div>
</template>

<script>
export default {
  props: {
    text: String,
    large: Boolean,
    extraClass: String
  }
}
</script>

<style scoped>
</style>