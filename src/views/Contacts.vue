<template>
  <div class="contacs">
    <h1>This is an contacts page</h1>
    <router-link to="/contacts/1">Contacts 1</router-link> |
    <router-link to="/contacts/2">Contacts 2</router-link>
    <h2>Contacts number is {{ id }}</h2>
    <button @click="toUser">User 1 のページへ</button>
  </div>
</template>

<script>
export default {
  props: ['id'],
  methods: {
    toUser () {
      this.$router.push('/users/1')
    }
  }
}
</script>
