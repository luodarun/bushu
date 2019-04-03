<template>
  <div>
    <button @click="test">点我一下试试</button>
  </div>
</template>
<script>
export default {
  name: 'my-button',
  data () {
    return {}
  },
  methods: {
    test () {
      this.$http.request({
        method: 'post',
        url: '/upload',
        data: 131,
        headers: { 'Content-Type': 'multipart/form-data' }
      })
    }
  }
}
</script>
