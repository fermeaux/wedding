<template>
  <div :class="`${size === '16' ? 'w-16 h-16' : 'w-12 h-12'} flex justify-center items-center`">
    <img :src="imageUrl" :class="`${size === '16' ? 'max-w-16 max-h-16' : 'max-w-12 max-h-12'}`">
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
      default: 'dog.svg'
    },
    size: {
      type: String,
      default: '16'
    }
  },
  computed: {
    imageUrl () {
      return require(`~/assets/images/${this.image}`)
    }
  }
}
</script>
