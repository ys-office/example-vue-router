<template>
  <div class="about">
    <h1>This is an about page {{ message }}</h1>
  </div>
</template>

<script>

export default {
  props: ['message'],
  name: 'about'
}
</script>
