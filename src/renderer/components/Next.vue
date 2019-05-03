<template>
  <dev>
    <router-link to="/">Return to the landing page.</router-link>
  </dev>
</template>

<script>
  export default {
    name: 'next-page',
    methods: {
      open (link) {
        this.$electron.shell.openExternal(link)
      }
    }
  }
</script>
