<script setup lang="ts">
const runtimeConfig = useRuntimeConfig()
const appConfig = useAppConfig()
useSeoMeta({
  title: 'Chef pas de retard',
  ogTitle: 'Chef pas de retard',
  description: 'Chef pas de retard vous offre une expérience unique pour maîtriser le temps avec élégance. Découvrez notre sélection de billets de retards soigneusement conçus pour vous accompagner avec style à chaque étape de votre journée. Évitez les tracas liés aux retards et embrassez la ponctualité avec nos solutions créatives. Parce que dans le monde exigeant d\'aujourd\'hui, être en retard n\'est plus une option. Achetez votre billet maintenant et rejoignez la communauté des chefs de la ponctualité.',
  ogDescription: 'Chef pas de retard vous offre une expérience unique pour maîtriser le temps avec élégance. Découvrez notre sélection de billets de retards soigneusement conçus pour vous accompagner avec style à chaque étape de votre journée. Évitez les tracas liés aux retards et embrassez la ponctualité avec nos solutions créatives. Parce que dans le monde exigeant d\'aujourd\'hui, être en retard n\'est plus une option. Achetez votre billet maintenant et rejoignez la communauté des chefs de la ponctualité.',
  ogImage: 'https://example.com/image.png',
  twitterCard: 'summary_large_image',
})
</script>

<template>
      <NuxtPage />
</template>

<style lang="scss">
@use "~/assets/scss/main.scss";
</style>