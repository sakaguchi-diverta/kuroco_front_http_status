<template>
  <div>Not found. (nuxt template)</div>
</template>

<script>
export default {
  name: '404Page',
  data() {
    return {
      meta: {
        title: `Not found.`,
        description: `Not found... `,
      },
    }
  },
  head() {
    return {
      title: this.meta.title || false,
      meta: [
        {
          hid: 'title',
          name: 'title',
          content: this.meta.title || false,
        },
        {
          hid: 'description',
          name: 'description',
          content: this.meta.description || false,
        },
        {
          hid: 'og:title',
          property: 'og:title',
          content: this.meta.title || false,
        },
        {
          hid: 'og:description',
          property: 'og:description',
          content: this.meta.description || false,
        },
        {
          hid: 'twitter:title',
          name: 'twitter:title',
          content: this.meta.title || false,
        },
        {
          hid: 'twitter:description',
          property: 'twitter:description',
          content: this.meta.description || false,
        },
      ],
    }
  },
}
</script>
