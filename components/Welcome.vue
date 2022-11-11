<template>
  <section class="min-h-screen flex flex-col justify-center items-center relative text-center">
    <h2
      data-wow-duration="2s"
      class="font-gistesy text-6xl text-tumbleweed pb-8 wow fadeInUp"
    >
      Reservez la date,<br>on se marie !
    </h2>
    <h1
      data-wow-delay="0.5s"
      data-wow-duration="2s"
      class="font-blackmango text-6xl text-wenge text-center wow fadeInUp"
    >
      Timothée & Manon
    </h1>
    <p
      data-wow-delay="1s"
      data-wow-duration="2s"
      class="font-forum text-2xl text-wenge wow fadeInUp"
    >
      16 SEPTEMBRE 2023
    </p>
    <div
      data-wow-delay="1.5s"
      data-wow-duration="2s"
      class="wow fadeInUp"
    >
      <button
        data-wow-delay="3.5s"
        data-wow-duration="1s"
        class="font-blackmango text-xl text-floral-white px-8 py-6 mt-16 cursor bg-full bg-cta z-10 wow swing"
        @click="confirm"
      >
        VEUILLEZ CONFIRMER
      </button>
    </div>
    <img src="~/assets/images/flowers.png" class="absolute top-0 left-0 max-w-xxs max-h-xxs md:max-w-lg md:max-h-lg z-deco">
    <img src="~/assets/images/flowers.png" class="absolute bottom-0 right-0 max-w-xxs max-h-xxs md:max-w-lg md:max-h-lg rotate-180 transform z-deco">
  </section>
</template>

<script>
export default {
  methods: {
    confirm () {
      document.getElementById('contact').scrollIntoView({ behavior: 'smooth', block: 'end', inline: 'nearest' })
    }
  }
}
</script>
