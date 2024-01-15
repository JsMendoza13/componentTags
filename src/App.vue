<script>
import InputTags from './components/InputTags.vue'

export default {
  components: {
    InputTags
  },
  methods: {
    handleOnTagsChange(tags) {
      console.log(tags)
    }
  }
}
</script>

<template>
  <h1>Agrega Tags</h1>
  <section>
    <InputTags @onTagsChange="handleOnTagsChange" />
  </section>
</template>

<style scoped>
section {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}

h1 {
  text-align: center;
}
</style>
