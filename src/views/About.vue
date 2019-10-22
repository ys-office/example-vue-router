<template>
  <div class="about">
    <h1>This is an about page {{ message }}</h1>
    <h2>{{ message_from_data_from_props_from_about_view }}</h2>
  </div>
</template>

<script>

export default {
  props: ['message'],
  name: 'about',
  data () {
    return {
      message_from_data_from_props_from_about_view: this.message
    }
  }
}
</script>
