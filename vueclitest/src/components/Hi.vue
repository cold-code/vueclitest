<template>
    <div>
        <h2>{{ msg }}</h2>
        <router-view/>
    </div>
</template>
<script>
export default {
  name: 'Hi1',
  data () {
    return {
      msg: 'Welcome to My Hi page,I am Coldcode'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
