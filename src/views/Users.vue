<template>
  <div class="users">
    <h1>This is an users page</h1>
    <router-link to="/users/1">User 1</router-link> |
    <router-link to="/users/2">User 2</router-link>
    <h2>User number is {{ id }}</h2>
    <button @click="toAbout">About ページへ</button>
  </div>
</template>

<script>
export default {
  props: ['id'],
  methods: {
    toAbout () {
      // this.$router.push('about')
      this.$router.push({ name: 'about', params: { message: 'Hello' } })
    }
  }
}
</script>
