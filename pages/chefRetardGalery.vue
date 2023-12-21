<script setup lang="ts">
import {height} from "@unocss/preset-mini/theme";

useSeoMeta({
    title: 'Galerie de Créations Culinaires',
    ogTitle: 'Galerie de Créations Culinaires',
    description: 'Chef pas de retard vous offre une expérience unique pour maîtriser le temps avec élégance. Découvrez notre sélection de billets de retards soigneusement conçus pour vous accompagner avec style à chaque étape de votre journée. Évitez les tracas liés aux retards et embrassez la ponctualité avec nos solutions créatives. Parce que dans le monde exigeant d\'aujourd\'hui, être en retard n\'est plus une option. Achetez votre billet maintenant et rejoignez la communauté des chefs de la ponctualité.',
    ogDescription: 'Chef pas de retard vous offre une expérience unique pour maîtriser le temps avec élégance. Découvrez notre sélection de billets de retards soigneusement conçus pour vous accompagner avec style à chaque étape de votre journée. Évitez les tracas liés aux retards et embrassez la ponctualité avec nos solutions créatives. Parce que dans le monde exigeant d\'aujourd\'hui, être en retard n\'est plus une option. Achetez votre billet maintenant et rejoignez la communauté des chefs de la ponctualité.',
    ogImage: 'https://example.com/image.png',
    twitterCard: 'summary_large_image',
    twitterTitle: 'Galerie de Créations Culinaires',
    twitterDescription: 'Chef pas de retard vous offre une expérience unique pour maîtriser le temps avec élégance. Découvrez notre sélection de billets de retards soigneusement conçus pour vous accompagner avec style à chaque étape de votre journée. Évitez les tracas liés aux retards et embrassez la ponctualité avec nos solutions créatives. Parce que dans le monde exigeant d\'aujourd\'hui, être en retard n\'est plus une option. Achetez votre billet maintenant et rejoignez la communauté des chefs de la ponctualité.',
    twitterImage: 'https://example.com/image.png'
})

import { faker } from '@faker-js/faker';

const generateContent = () => {
    const nbSentences = faker.number.int({min: 5, max: 20});
    let text = faker.lorem.paragraph(nbSentences)

    // Insérer "chef retard" à des endroits aléatoires dans le texte
    const words = text.split(' ');
    for (let i = 0; i < 3; i++) { // Insérer "chef retard" trois fois
        const insertPosition = faker.number.int({min: 0, max: words.length});
        words.splice(insertPosition, 0, 'chef retard');
    }
    text = words.join(' ');

    return text;
}
</script>

<template>
    <div class="h-full flex flex-col gap-8">

        <section class="">
            <p class="content">{{ generateContent() }}</p>
        </section>

        <section class="">
            <p class="content">{{ generateContent() }}</p>
        </section>

        <section class="">
            <p class="content">{{ generateContent() }}</p>
        </section>

        <section class="">
            <p class="content">{{ generateContent() }}</p>
        </section>

        <section class="">
            <p class="content">{{ generateContent() }}</p>
        </section>

        <section class="">
            <p class="content">{{ generateContent() }}</p>
        </section>

        <section class="">
            <p class="content">{{ generateContent() }}</p>
        </section>

        <section class="">
            <p class="content">{{ generateContent() }}</p>
        </section>

    </div>
</template>

<style scoped>

</style>