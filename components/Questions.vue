<template>
  <section class="relative min-h-screen py-16 lg:py-32 px-16 flex">
    <div class="w-full lg:w-1/2 lg:pr-8">
      <h1 class="font-gistesy text-7xl text-tumbleweed text-center block pb-4 lg:hidden">
        Questions / Reponses
      </h1>
      <div v-for="topic in topics" :key="topic.question" class="py-4">
        <h2 class="font-forum text-xl text-wenge">
          {{ topic.question }}
        </h2>
        <p class="font-forum text-xl text-tumbleweed">
          {{ topic.answer }}
        </p>
      </div>
    </div>
    <div class="hidden lg:w-1/2 lg:pl-8 lg:flex-col lg:items-center lg:flex">
      <h1 class="font-gistesy text-7xl text-tumbleweed text-center">
        Questions / Reponses
      </h1>
      <img data-wow-delay="0.5s" src="~/assets/images/pot.png" class="h-96 pt-8  wow bounceInRight">
    </div>
    <BackgroundFloral />
  </section>
</template>

<script>
export default {
  data () {
    return {
      topics: [
        {
          question: "Peut-on réserver ailleurs  qu'à l'hôtel 7Hotel&Spa ?",
          answer: "À proximité il y a aussi : Appart'hôtel Adagio Access, Hôtel restaurant d'Alsace The Originals Boutique, Holiday Inn Express, Hôtel Restaurant Campanile,  B&B HOTEL,  Ibis Budget."
        },
        {
          question: 'Quand devrions-nous être là ?',
          answer: "La cérémonie aura lieu le 16 septembre, alors veuillez planifier votre voyage en conséquence. Vous pouvez choisir d'arriver avant le jour même pour profiter du spa de l'hôtel ou visiter Strasbourg !"
        },
        {
          question: 'Et en tram,  ça donne quoi ?',
          answer: "L'arrêt le plus proche est \"Campus d'Illkirch\" (12 minutes à pied jusqu'à l'hôtel)."
        }
      ]
    }
  }
}
</script>
