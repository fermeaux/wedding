<template>
  <div :data-wow-delay="delayAnimation" :class="`flex flex-col items-center w-32 wow bounceInUp ${iconSize === '24' ? 'mx-m8' : 'mx-m10'}`">
    <Icon :image="image" :size="iconSize" />
    <p :class="`${textSize === 'lg' ? 'text-lg' : 'text-2xl'} font-forum text-tumbleweed text-center pt-2`">
      {{ date }}
    </p>
    <h2 :class="`${textSize === 'lg' ? 'text-lg' : 'text-2xl'} font-forum text-tumbleweed text-center`">
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
    },
    textSize: {
      type: String,
      default: 'lg'
    },
    iconSize: {
      type: String,
      default: '16'
    },
    delayAnimation: {
      type: String,
      default: '0s'
    }
  }
}
</script>
