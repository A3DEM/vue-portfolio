<template>
    <div id="design-projects">
        <TitleComp title="Projets graphisme" overlay="Projets graphisme"/>

        <div v-for="project in projects" v-bind:key="project" class="project-comp">
            <h3>{{project.title}}</h3>
            <p>{{project.paragraph}}</p>
            <LinkButton/>
        </div>
    </div>
</template>

<script>

import TitleComp from './TitleComp.vue'
import LinkButton from './LinkButton.vue';

export default {
    name: "DesignProjects",
    components: {
    TitleComp,
    LinkButton
},
    data() {
        return {
            projects: [
                {
                    title: "Euro 2021",
                    paragraph: "À l’occasion de l’Euro 2021, j’ai produit une affiche pour le match France-Suisse."
                },
                {
                    title: "WHISTLE",
                    paragraph: "Étant un grand fan de football, j’ai imaginé le logo d’un réseau social pour fans. À long terme, mon projet serait de designer l’interface de cette application et de la développer !"
                },
                {
                    title: "WATERMELON STUDIO",
                    paragraph: "Dans le cadre d’un projet en module d’anglais, nous avons dû créer une agence fictive. Voici l’identité graphique de cette dernière."
                },
                {
                    title: "MAISON ALSACIENNE DE BISCUITERIE",
                    paragraph: "Dans le cadre d’un projet en module d’anglais, nous avons dû créer l’identité graphique de la Maison Alsacienne de Biscuiterie. Voici l’identité graphique de cette dernière."
                },
                {
                    title: "CARTE GOLD / CARTE NOIRE",
                    paragraph: "Originaire de la Courneuve, le rappeur Dinos a partagé deux titres avant la sortie de son premier album. Ces deux morceaux, respectivement Carte Gold et Carte Noire, servaient à faire la promotion de ce dernier. J’ai donc imaginé deux vraies cartes bancaires à l’effigie du rappeur."
                },
                {
                    title: "ULTRA",
                    paragraph: "Au cours de l’année 2021, le rappeur Booba a sorti son dernier album intitulé « Ultra ». Afin de célébrer la sortie de l’album, j’ai créé une pochette fictive du projet en 3D."
                },
                {
                    title: "BURAK « KRAL » YILMAZ",
                    paragraph: "Otto. C’est à travers ces quatre lettres que le rappeur SCH nous parle de son père dans ce titre, issu de son album JVLIVS. J’ai décidé de créer une pochette dans ce thème."
                },
                {
                    title: "nouvo mode",
                    paragraph: "Sorti le 6 mars, l’album Nouvo Mode de Sneazzy était l’un des projets que j’attendais le plus en 2020. Dès son annonce j’ai commencé à travailler sur la pochette que j’allais poster sur les réseaux."
                },
                {
                    title: "TRINITY",
                    paragraph: "C’est avec un style atypique que le rappeur Laylow s’est imposé dans l’industrie musicale. Avec son style digital, il a marqué l’année 2020 grâce à son projet TRINITY. Innovateur, l’album se veut être un « logiciel de stimulation émotionnelle ». J’ai décidé de créer une pochette pour TRINITY en m’inspirant du style unique de Laylow."
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
    #design-projects {
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