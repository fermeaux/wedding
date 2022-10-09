<template>
  <div :class="`w-${size} h-${size} flex justify-center items-center`">
    <img :src="imageUrl" :class="`max-w-${size} max-h-${size}`">
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
