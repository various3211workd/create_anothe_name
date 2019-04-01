<template>
  <div>
    {{ this.name }}
  </div>
</template>

<script>
export default {
  data () {
    return {
      name: ''
    }
  },
  methods: {
    CreateName() {
      this.name = 'test'
    },
  }
}
</script>

<style scoped>

</style>
