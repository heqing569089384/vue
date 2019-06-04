<template>
  <div class="hello">
    <p>
      <router-link to="/home">go to foo</router-link>
      <router-link  to="/user/123">User123</router-link>
      <router-link to="/user/456">User456</router-link>
    </p>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  data () {
    return {
     
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
