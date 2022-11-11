<template>
  <div :class="`${sizeClass} flex justify-center items-center`">
    <img :src="imageUrl" :class="`${sizeMaxClass}`">
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
    },
    isRing: {
      type: Boolean,
      default: false
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
      } else if (this.isRing && this.size === '8') {
        return 'w-12 h-8'
      } else if (this.size === '8') {
        return 'w-8 h-8'
      }
      return 'w-12 h-12'
    },
    sizeMaxClass () {
      if (this.size === '16') {
        return 'max-w-16 max-h-16'
      } else if (this.size === '24') {
        return 'max-w-24 max-h-16'
      } else if (this.isRing && this.size === '8') {
        return 'max-w-12 max-h-8'
      } else if (this.size === '8') {
        return 'max-w-8 max-h-8'
      }
      return 'max-w-12 max-h-12'
    }
  }
}
</script>
