<template>
  <section class="container">
    <div>
      <!-- <app-logo/> -->
      <h2 class="subtitle">
        作成された名前は
      </h2>
      <h1 class="title">
        <create-name ref="cname"></create-name>
      </h1>
      <h2 class="subtitle">
        です！
      </h2>
      <button 
         v-on:click="callCreateName()" 
        class="button--green">Create</button>
    </div>
  </section>
</template>

<script>
import CreateName from '~/components/CreateName.vue'

export default {
  components: {
    CreateName
  },
  /*
  data() {
    return {
    }
  },
  */
  methods: {
    callCreateName() {
      this.$refs.cname.CreateName()
    }
  },
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

