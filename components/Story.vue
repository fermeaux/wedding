<!-- eslint-disable vue/valid-v-for -->
<template>
  <section class="min-h-screen relative">
    <h1 class="font-gistesy text-6xl text-tumbleweed ml-8 mt-8 md:ml-16 md:mt-16 relative inline-block leading-tight">
      Notre belle<br>histoire d'amour
      <img src="~/assets/images/arrow.png" class="absolute bottom-1/3 left-1/3 w-full h-1/2 transform rotate-18">
    </h1>
    <div class="hidden md:flex absolute top-1/2 left-1/2 w-full transform translate-x-m1/2 translate-y-m1/2 flex-row justify-center items-start">
      <template v-for="(step, index) in steps">
        <StepDivider v-if="index > 0" />
        <StepItem
          :image="step.image"
          :label="step.label"
          :date="step.date"
          :text-size="step.textSize || 'lg'"
          :icon-size="step.iconSize || '16'"
        />
      </template>
    </div>
    <div class="flex md:hidden absolute top-1/2 left-1/2 transform translate-x-m1/2 translate-y-m1/2 flex-col justify-center items-start">
      <template v-for="step in steps">
        <StepItemMobile
          :image="step.image"
          :label="step.label"
          :date="step.date"
        />
      </template>
    </div>
    <BackgroundFloral />
  </section>
</template>

<script>
export default {
  data () {
    return {
      steps: [
        {
          image: 'heart.svg',
          label: 'Premier baiser',
          date: '07/06/2016'
        },
        {
          image: 'house.png',
          label: 'Premier appart',
          date: '01/09/2017'
        },
        {
          image: 'ring.png',
          label: 'La demande (Enfin !)',
          date: '10/10/2020'
        },
        {
          image: 'dog.svg',
          label: 'Le petit chien',
          date: '01/12/2021'
        },
        {
          image: 'double-ring.png',
          label: 'Le mariage',
          date: '16/09/2023',
          textSize: '2xl',
          iconSize: '24'
        }
      ]
    }
  }
}
</script>
