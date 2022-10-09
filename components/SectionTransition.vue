<template>
  <div :class="`h-${size} bg-gradient-to-${direction} from-white to-floral-white z-bg my-m${size / 2}`" />
</template>

<script>
export default {
  props: {
    direction: {
      type: String,
      default: 'b'
    },
    size: {
      type: Number,
      default: 16
    }
  }
}
</script>
