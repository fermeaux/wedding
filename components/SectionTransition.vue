<template>
  <div :class="`${direction === 'b' ? 'bg-gradient-to-b' : 'bg-gradient-to-t'} h-16 from-white to-floral-white z-bg my-m8`" />
</template>

<script>
export default {
  props: {
    direction: {
      type: String,
      default: 'b'
    }
  }
}
</script>
