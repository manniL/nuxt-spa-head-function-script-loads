<template>
  <h1>Please check the console!</h1>
</template>

<script>
export default {
  head() {
    return {
      script: [
        {
          innerHTML: 'console.log(`head components/Logo.vue`)'
        }
      ]
    }
  },
  mounted() {
    console.log(`Logo.vue mounted`)
  }
}
</script>
