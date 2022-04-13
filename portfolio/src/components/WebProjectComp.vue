<template>
    <div v-for="project in projects" v-bind:key="project" class="project">
        <h3>{{project.title}}</h3>
        <p>{{project.paragraph}}</p>
        <div class="links">
            <LinkComp link="{{project.links.demo}}" title="Voir le projet"/>
            <LinkComp title="Voir le code source"/>
        </div>
    </div>
</template>

<script>
import LinkComp from "./LinkComp.vue"

    export default {
        name:"WebProjectComp",
        components: {
            LinkComp,
        },
            data() {
        return {
            projects: [
                {
                    title: "Tesla",
                    paragraph: "J’ai un intérêt pour l’automobile. Dans ce projet, j’ai intégré une maquette servant de page de présentation des véhicules Tesla. L’animation est faite grâce à GSAP.",
                    links: [{
                        demo: "https://www.perdu.com",
                        sourceCode: "https://www.perdu.com"
                    }]
                },
                {
                    title: "BMW M4",
                    paragraph: "Dans ce projet, j’ai imaginé une page de présentation pour la BMW M4. J’ai voulu particulièrement soigné le chargement. J’ai pu utiliser la librairie GSAP pour l’animation."
                },
                {
                    title: "Mocha Café",
                    paragraph: "Lors de ma recherche de stage de 2ème année, j’ai effectué des tests au sein de l’entreprise Numendo. Je devais reproduire une maquette autour de la thématique du café."
                },
                {
                    title: "Les cartes projets",
                    paragraph: "Lors du développement de mon portfolio, j’ai décidé de créer des cartes projets personnalisés. Voici le résultat ! J’ai également ajouté un effet de mouvement dans la première carte en utilisant la libraire tilt.js."
                },
                {
                    title: "Matrix",
                    paragraph: "À l’occasion de la sortie du dernier film Matrix, j’ai tenté de créer une page qui reprend la direction artistique du 4ème volet de la saga."
                },
                {
                    title: "Calculatrice de matrices",
                    paragraph: "Afin de vérifier mes calculs pour mon module de maths pour le web, j’ai codé une calculatrice de matrices, qui permet d’effectuer un produit matriciel."
                },
                {
                    title: "Fonctions mathématiques",
                    paragraph: "Dans le cadre du module de mathématiques, j’ai été en charge de développer plusieurs fonctions mathématiques. Ce projet de première année permet de calculer le PGCD, le PPCM, les coefficients de Bézout ainsi que la factorisation en nombres premiers pour deux nombres donnés mais également de chiffrer votre message selon le décalage que vous souhaitez."
                },
                {
                    title: "Mercedes-Benz",
                    paragraph: "J’ai décidé de créer une page d’accueil pour le site web de Mercedes-Benz d’après une maquette trouvée sur Dribbble."
                },
                {
                    title: "Ancien portfolio Angular",
                    paragraph: "Accompagné d’un ingénieur études et développement de SFEIR Strasbourg, j’ai pu créer mon portfolio sous Angular en reprenant un thème HTML pré-construit. Le principal objectif de ce projet était de mieux connaître l’environnement Angular."
                },
                {
                    title: "Switch Jour-Nuit",
                    paragraph: "Jouez avec le switch pour découvir ce qu’il déclenche !"
                },
            ]
        }
    },
    }
</script>

<style lang="scss" scoped>
.project {
    h3 {
        font-size: 16px;
        font-weight: normal;
    }
    p {
        font-size: 12px;
        margin-top: 10px;
        margin-bottom: 0;
        color: #6D6D6D;
    }
    .links {
        margin-top: 10px;
    }
}
</style>