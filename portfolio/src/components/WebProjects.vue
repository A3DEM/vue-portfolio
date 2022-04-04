<template>
    <div id="web-projects">
        <TitleComp title="Projets web" overlay="Projets web"/>

        <div v-for="project in projects" v-bind:key="project" class="project-comp">
            <h3>{{project.title}}</h3>
            <p>{{project.paragraph}}</p>
            <LinkButton/>
        </div>
    </div>
</template>

<script>

import TitleComp from './TitleComp.vue'
// import ButtonComp from "./ButtonComp.vue";
import LinkButton from './LinkButton.vue';

export default {
    name: "WebProjects",
    components: {
    TitleComp,
    // ButtonComp,
    LinkButton
},
    data() {
        return {
            projects: [
                {
                    title: "Tesla",
                    paragraph: "J’ai un intérêt pour l’automobile. Dans ce projet, j’ai intégré une maquette servant de page de présentation des véhicules Tesla. L’animation est faite grâce à GSAP."
                },
                {
                    title: "BMW M4",
                    paragraph: "Dans ce projet, j’ai imaginé une page de présentation pour la BMW M4. J’ai voulu particulièrement soigné le chargement. J’ai pu utiliser la librairie GSAP pour l’animation."
                },
                {
                    title: "MOCHA CAFÉ",
                    paragraph: "Lors de ma recherche de stage de 2ème année, j’ai effectué des tests au sein de l’entreprise Numendo. Je devais reproduire une maquette autour de la thématique du café."
                },
                {
                    title: "LES CARTES PROJETS",
                    paragraph: "Lors du développement de mon portfolio, j’ai décidé de créer des cartes projets personnalisés. Voici le résultat ! J’ai également ajouté un effet de mouvement dans la première carte en utilisant la libraire tilt.js."
                },
                {
                    title: "matrix",
                    paragraph: "À l’occasion de la sortie du dernier film Matrix, j’ai tenté de créer une page qui reprend la direction artistique du 4ème volet de la saga."
                },
                {
                    title: "CALCULATRICE DE MATRICES",
                    paragraph: "Afin de vérifier mes calculs pour mon module de maths pour le web, j’ai codé une calculatrice de matrices, qui permet d’effectuer un produit matriciel."
                },
                {
                    title: "FONCTIONS MATHÉMATIQUES",
                    paragraph: "Dans le cadre du module de mathématiques, j’ai été en charge de développer plusieurs fonctions mathématiques. Ce projet de première année permet de calculer le PGCD, le PPCM, les coefficients de Bézout ainsi que la factorisation en nombres premiers pour deux nombres donnés mais également de chiffrer votre message selon le décalage que vous souhaitez."
                },
                {
                    title: "MERCEDES-BENZ",
                    paragraph: "J’ai décidé de créer une page d’accueil pour le site web de Mercedes-Benz d’après une maquette trouvée sur Dribbble."
                },
                {
                    title: "ANCIEN PORTFOLIO ANGULAR",
                    paragraph: "Accompagné d’un ingénieur études et développement de SFEIR Strasbourg, j’ai pu créer mon portfolio sous Angular en reprenant un thème HTML pré-construit. Le principal objectif de ce projet était de mieux connaître l’environnement Angular."
                },
                {
                    title: "SWITCH JOUR-NUIT",
                    paragraph: "Jouez avec le switch pour découvir ce qu’il déclenche !"
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
    #web-projects {
        margin: 35px 0px 20px 0px;
        text-align: left;

        h3 {
            text-transform: uppercase;
            font-size: 24px;
            margin-bottom: 10px;
            margin-top: 35px;
            font-style: italic;
        }
        p {
            font-family: poppins, sans-serif;
            font-size: 14px;
            margin-bottom: 25px;
        }
    }
</style>