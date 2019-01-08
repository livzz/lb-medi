<template>
  <div class="mx-auto" :class="{'siteContent' : !inner, 'innerSiteContent': inner}">
    <slot></slot>
  </div>
</template>

<script>
export default {
  props: {
    inner: Boolean
  }
}
</script>

<style>
.siteContent {
  max-width: 1470px;
}

.innerSiteContent {
  max-width: 1300px;
}
</style>