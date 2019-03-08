<template>
  <div>
    <h1>Event #{{ id }}</h1>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: 'ECreate ' + this.id,
      meta: [
        {
          hid: 'desciption',
          name: 'description',
          content: 'Creatin a new event ' + this.id
        }
      ]
    }
  },
  computed: {
    id() {
      return this.$route.params.id
    }
  }
}
</script>
