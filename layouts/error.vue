<template>
  <div>
    <h1 v-if="error.statusCode === 404">Page not found</h1>
    <h1 v-else>An error occurred</h1>
    <NuxtLink to="/">Home page</NuxtLink>
  </div>
</template>

<script>
export default {
  layout: 'error',
  props: {
    error: {
      type: Object,
      default() {
        return {}
      },
    },
  },
  head() {
    return {
      title: 'Err Title',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Err Desc',
        },
      ],
    }
  },
}
</script>
