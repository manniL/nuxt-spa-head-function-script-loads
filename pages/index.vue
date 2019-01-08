<template>
  <div class="container"><test /></div>
</template>

<script>
import Test from '~/components/Logo'
export default {
  components: { Test },
  head() {
    return {
      script: [
        {
          innerHTML: 'console.log(`head pages/index.vue`)'
        },
        {
          innerHTML: 'console.log(`head pages/index.vue with body: true`)',
          body: true
        }
      ]
    }
  },
  mounted() {
    console.log(`index.vue mounted`)
  }
}
</script>

<style scoped>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
h1 {
  font-weight: 400;
}
.name {
  color: #3b8070;
}
p {
  margin-top: 20px;
}
</style>
