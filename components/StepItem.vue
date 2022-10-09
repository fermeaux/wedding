<template>
  <div class="flex flex-col items-center w-32 mx-m10">
    <Icon :image="image" :size="imageSize" />
    <p :class="`text-${textSize} font-forum text-tumbleweed text-center pt-2`">
      {{ date }}
    </p>
    <h2 :class="`text-${textSize} font-forum text-tumbleweed text-center`">
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
    imageSize: {
      type: String,
      default: '16'
    },
    label: {
      type: String,
      default: 'Le mariage'
    },
    date: {
      type: String,
      default: '16/09/2023'
    },
    textSize: {
      type: String,
      default: 'xl'
    }
  }
}
</script>
