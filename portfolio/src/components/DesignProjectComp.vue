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
                    title: "Euro 2021",
                    paragraph: "À l’occasion de l’Euro 2021, j’ai produit une affiche pour le match France-Suisse."
                },
                {
                    title: "Whistle",
                    paragraph: "Étant un grand fan de football, j’ai imaginé le logo d’un réseau social pour fans. À long terme, mon projet serait de designer l’interface de cette application et de la développer !"
                },
                {
                    title: "Watermelon Studio",
                    paragraph: "Dans le cadre d’un projet en module d’anglais, nous avons dû créer une agence fictive. Voici l’identité graphique de cette dernière."
                },
                {
                    title: "Maison Alsacienne de Biscuiterie",
                    paragraph: "Dans le cadre d’un projet en module d’anglais, nous avons dû créer l’identité graphique de la Maison Alsacienne de Biscuiterie. Voici l’identité graphique de cette dernière."
                },
                {
                    title: "Carte Gold | Carte Noire",
                    paragraph: "Originaire de la Courneuve, le rappeur Dinos a partagé deux titres avant la sortie de son premier album. Ces deux morceaux, respectivement Carte Gold et Carte Noire, servaient à faire la promotion de ce dernier. J’ai donc imaginé deux vraies cartes bancaires à l’effigie du rappeur."
                },
                {
                    title: "Ultra",
                    paragraph: "Au cours de l’année 2021, le rappeur Booba a sorti son dernier album intitulé « Ultra ». Afin de célébrer la sortie de l’album, j’ai créé une pochette fictive du projet en 3D."
                },
                {
                    title: "Burak « Kral » Yilmaz",
                    paragraph: "Otto. C’est à travers ces quatre lettres que le rappeur SCH nous parle de son père dans ce titre, issu de son album JVLIVS. J’ai décidé de créer une pochette dans ce thème."
                },
                {
                    title: "Otto",
                    paragraph: "Otto. C’est à travers ces quatre lettres que le rappeur SCH nous parle de son père dans le titre éponyme, issu de son album JVLIVS. L’illustration a pour but d’être une pochette pour le morceau."
                },
                {
                    title: "Nouvo Mode",
                    paragraph: "Sorti le 6 mars, l’album Nouvo Mode de Sneazzy était l’un des projets que j’attendais le plus en 2020. Dès son annonce j’ai commencé à travailler sur la pochette que j’allais poster sur les réseaux."
                },
                {
                    title: "Project Resident Evil 2",
                    paragraph: "Propulsé sur Orion, une console fictive, redécouvrez Resident Evil 2, un jeu d'horreur sorti en 1998 et réadapté en 2019. Après avoir eu une très bonne expérience avec la version sortie en 2019, j'ai décidé de créer des modèles 3D des armes de Leon S. Kennedy (l'un des personnages principaux) et d’autres éléments du jeu."
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