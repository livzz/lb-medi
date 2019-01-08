<template>
  <div class="topHeader w-full mt-8">
    <div v-if="logoText">
      <div class="logo mx-auto flex items-center justify-center">
        <div>
          <img src="~/assets/img/group.png" alt>
        </div>
      </div>
      <h2 class="text-center name-color">Medi Service Pvt. Ltd.</h2>
    </div>
    <nav class="nav flex justify-center md:flex-no-wrap flex-wrap mt-8">
      <a
        :href="data.link"
        v-for="(data,i) in navData"
        :key="i"
        class="mx-4 xxl:mx-20 xl:mx-16 lg:mx-8 xl:text-2xl text-lg"
      >{{data.name}}</a>
    </nav>
  </div>
</template>

<script>
export default {
  props: {
    noOfLinks: Number,
    links: Object,
    navData: Array,
    logoText: String,
    logoSubtitle: String
  }
}
</script>

<style scoped>
a {
  text-decoration: none;
  color: black;
}
</style>