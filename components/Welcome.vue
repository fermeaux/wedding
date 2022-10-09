<template>
  <section class="min-h-screen flex flex-col justify-center items-center relative text-center">
    <h2 class="font-gistesy text-6xl text-tumbleweed pb-8">
      Reservez la date
    </h2>
    <h1 class="font-blackmango text-6xl text-wenge text-center">
      Timothée & Manon
    </h1>
    <p class="font-forum text-2xl text-wenge">
      16 SEPTEMBRE 2023
    </p>
    <button
      class="font-blackmango text-xl text-floral-white px-8 py-6 mt-16 cursor bg-full bg-cta z-10"
      @click="confirm"
    >
      VEUILLEZ CONFIRMER ICI
    </button>
    <img src="~/assets/images/flowers.png" class="absolute top-0 left-0 max-w-lg max-h-lg z-deco">
    <img src="~/assets/images/flowers.png" class="absolute bottom-0 right-0 max-w-lg max-h-lg rotate-180 transform z-deco">
  </section>
</template>

<script>
export default {
  methods: {
    confirm () {
      alert("Cette fonctionnalité n'est pas encore disponible")
    }
  }
}
</script>
