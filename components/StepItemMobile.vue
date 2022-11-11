<template>
  <div :class="`flex flex-row items-center py-2 ${isRing ? 'ml-m4': ''} w-76`">
    <Icon :image="image" size="8" :is-ring="isRing" />
    <p class="text-lg font-forum text-tumbleweed text-center pl-4">
      {{ date }}
    </p>
    <p class="text-lg font-forum text-tumbleweed text-center pl-2">
      -
    </p>
    <h2 class="text-lg font-forum text-tumbleweed text-center pl-2">
      {{ label }}
    </h2>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
      default: 'dog.svg'
    },
    label: {
      type: String,
      default: 'Le mariage'
    },
    date: {
      type: String,
      default: '16/09/2023'
    }
  },
  computed: {
    isRing () {
      return this.date === '16/09/2023'
    }
  }
}
</script>
