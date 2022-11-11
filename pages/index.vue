<template>
  <main>
    <template v-if="isWowLoaded">
      <Welcome />
      <Important />
      <SectionTransition />
      <Story />
      <SectionTransition direction="t" />
      <Informations />
      <SectionTransition />
      <Questions />
      <SectionTransition direction="t" />
      <Contact />
    </template>
  </main>
</template>

<script>
export default {
  data () {
    return {
      isWowLoaded: false
    }
  },
  head () {
    return {
      script: [
        {
          hid: 'wow',
          src: '/js/wow.min.js',
          callback: () => {
            // eslint-disable-next-line no-undef
            const wow = new WOW()
            wow.init()
            this.isWowLoaded = true
          }
        }
      ]
    }
  }
}
</script>
