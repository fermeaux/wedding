<template>
  <section class="min-h-screen relative">
    <h1 class="font-gistesy text-7xl text-tumbleweed pt-32 text-center z-20">
      Programme
    </h1>
    <div class="flex flex-col md:flex-row justify-center pt-8">
      <div class="flex flex-col justify-center items-center text-center mb-8 md:mb-0">
        <span data-wow-delay="0.5s" data-wow-duration="2s" class="wow flipInX">
          <Icon image="church.png" size="32" />
        </span>
        <h2 class="font-gistesy text-5xl text-tumbleweed pt-4">
          16h00
        </h2>
        <div class="flex flex-col justify-center items-center text-center mx-m32 pt-2">
          <h2 class="font-blackmango text-xl text-dark-pastel-red pb-2">
            Paroisse protestante
          </h2>
          <p class="font-forum text-xl text-tumbleweed">
            3 Rue de l'église
          </p>
          <p class="font-forum text-xl text-tumbleweed">
            67115 Plobsheim
          </p>
        </div>
      </div>
      <div class="h-0 w-32 border-t-2 border-dotted border-tumbleweed md:mt-16 self-center md:self-start" />
      <div class="flex flex-col justify-center items-center mt-8 md:mt-0 mb-32 md:mb-0">
        <div class="flex flex-row">
          <div class="text-center">
            <span data-wow-delay="1.5s" data-wow-duration="2s" class="wow flipInX">
              <Icon image="glasses.png" size="32" />
            </span>
            <h2 class="font-gistesy text-5xl text-tumbleweed pt-4">
              17h30
            </h2>
          </div>
          <div class="h-0 w-32 border-t-2 border-dotted border-tumbleweed mt-16 hidden md:block" />
          <div class="text-center ml-4 md:ml-0">
            <span data-wow-delay="2.5s" data-wow-duration="2s" class="wow flipInX">
              <Icon image="cake.png" size="32" />
            </span>
            <h2 class="font-gistesy text-5xl text-tumbleweed pt-4">
              19h00
            </h2>
          </div>
        </div>
        <div class="flex flex-col md:flex-row justify-center items-center">
          <div class="flex flex-col justify-center items-center text-center pt-2">
            <h2 class="font-blackmango text-xl text-dark-pastel-red pb-2">
              7Hotel&Spa
            </h2>
            <p class="font-forum text-xl text-tumbleweed">
              550 Bd Sébastien Brant
            </p>
            <p class="font-forum text-xl text-tumbleweed">
              67400 Illkirch-Graffenstaden
            </p>
          </div>
        </div>
      </div>
    </div>
    <img src="~/assets/images/flowers.png" class="absolute top-0 left-0 max-w-xxs max-h-xxs md:max-w-lg md:max-h-lg z-none">
    <img src="~/assets/images/flowers.png" class="absolute bottom-0 right-0 max-w-xxs max-h-xxs md:max-w-lg md:max-h-lg rotate-180 transform z-10">
  </section>
</template>
