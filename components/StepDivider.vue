<template>
  <img :data-wow-delay="delayAnimation" src="~/assets/images/step.svg" class="w-32 h-16 px-6 wow bounceInUp">
</template>

<script>
export default {
  props: {
    delayAnimation: {
      type: String,
      default: '0s'
    }
  }
}
</script>
