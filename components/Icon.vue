<template>
  <div :class="`${sizeClass} flex justify-center items-center`">
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
    },
    sizeClass () {
      if (this.size === '16') {
        return 'w-16 h-16'
      } else if (this.size === '24') {
        return 'w-24 h-16'
      }
      return 'w-12 h-12'
    },
    sizeMaxClass () {
      if (this.size === '16') {
        return 'max-w-16 max-h-16'
      } else if (this.size === '24') {
        return 'max-w-24 max-h-16'
      }
      return 'max-w-12 max-h-12'
    }
  }
}
</script>
