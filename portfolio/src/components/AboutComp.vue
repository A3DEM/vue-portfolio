<template>
    <div id="about-me">
        <h2>À propos</h2>
        <p>Fan de football, curieux et polyvalent, je suis étudiant en Licence professionnelle en Webdesign-Webdéveloppement ainsi qu’en alternance au sein de l’agence <LinkComp class="no-margin" title="Première Place" link="https://premiere.place/"/> à Mulhouse ! </p>
        <p>Actuellement, je suis à la recherche d’une entreprise pour y effectuer mon mastère en Développement Web/Tech Lead chez Digital Campus Bordeaux.</p>
        <p>Découvrez ma personnalité, mon parcours et mes expériences à travers mon CV !</p>
        <LinkComp title="Télécharger le CV"/>
    </div>
</template>

<script>
import LinkComp from "./LinkComp.vue";
    export default {
    name: "TitleComp",
    components: { LinkComp }
}
</script>

<style lang="scss" scoped>
 #about-me {

    h2 {
        margin: 20px 0px 10px 0px
    }

    p {
        font-size: 12px;
        color: #6D6D6D;
        }
 }
</style>