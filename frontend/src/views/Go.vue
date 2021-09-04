<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <div>{{data}}</div>
  </div>
</template>

<script>
import post from '@/lib/post.js'
export default {
  created() {
    let params = new URLSearchParams()
    post("/test", params).then(res => {
      this.data = res.data
    })
  },
  name: 'Go',
  data() {
    return {
      data: {}
    }
  }
}
</script>