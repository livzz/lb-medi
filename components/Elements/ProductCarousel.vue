<template>
  <div>
    <carousel
      :perPage="1"
      class="mt-8"
      navigationEnabled
      :navigationPrevLabel="``"
      :navigationNextLabel="``"
    >
      <slide v-for="(data,i) in sliderData" :key="i">
        <div v-if="!alter">
          <div class="flex justify-center">
            <div class="flex-1">
              <div class="ml-auto">
                <img :src="data.image" alt="Hand woven" class="h-full w-full">
              </div>
            </div>
            <div class="flex-1 mr-8">
              <div class="w-3/5 mx-auto">
                <section-title :text="data.title"/>
                <section-subtitle class="mt-8" :text="data.description"/>
              </div>
            </div>
          </div>
        </div>
        <div v-else>
          <div class="flex justify-center">
            <div class="flex-1 mr-8">
              <div class="w-3/5 mx-auto">
                <section-title :text="data.title"/>
                <section-subtitle class="mt-8" :text="data.description"/>
              </div>
            </div>
            <div class="flex-1">
              <div class="ml-auto">
                <img :src="data.image" :alt="data.title" class="h-full w-full">
              </div>
            </div>
          </div>
        </div>
      </slide>
    </carousel>
  </div>
</template>

<script>
import SectionSubtitle from '~/components/Elements/SectionSubtitle'
import SectionTitle from '~/components/Elements/SectionTitle'

export default {
  components: {
    SectionSubtitle,
    SectionTitle
  },
  props: {
    sliderData: Array,
    alter: Boolean
  }
}
</script>

<style scoped>
</style>