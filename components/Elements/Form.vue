<template>
  <div class="main-form">
    <div class="form-bg form-bg-up w-full"></div>
    <div class="form-bg w-full"></div>
    <form class="form-container bg-white">
      <div class="form-input w-3/5 mx-auto">
        <input type="text" name="name" placeholder="Name" class="form-field px-4 py-4 w-full mb-4">
        <input
          type="text"
          name="email"
          placeholder="Email"
          class="form-field px-4 py-4 w-full mb-4"
        >
        <input
          type="text"
          name="phone"
          placeholder="Phone"
          class="form-field px-4 py-4 w-full mb-4"
        >
        <textarea
          name="query"
          id="form-query"
          cols="30"
          rows="8"
          placeholder="Query"
          class="form-field px-4 py-4 w-full mb-4"
        ></textarea>
      </div>
      <div class="text-center">
        <button class="px-16 py-4 border-2 border-black">Submit</button>
      </div>
    </form>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
$black: #000;

input {
  border-bottom: 2px solid $black;
  transition: all 0.2s ease-in;
  &:focus {
    border-bottom: 2px solid $black;
  }
}
textarea {
  border: 2px solid $black;
  transition: all 0.2s ease-in;
  &:focus {
    border: 2px solid $black;
  }
}
</style>