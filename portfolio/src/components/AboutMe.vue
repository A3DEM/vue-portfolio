<template>
    <div id="about-me">
        <TitleComp title="À propos" overlay="Qui suis-je ?"/>

        <p>Je suis Adem DURAN, 19 ans, étudiant en Licence professionnelle en Webdesign et en Webdéveloppement. Actuellement je suis en alternance chez Première Place !</p>
        <p>Fan de football, curieux et polyvalent, mon savoir-être et mon savoir-faire sont de réels atouts. Je vous propose vous pencher plus en détail sur ma personnalité, mon parcours et mes expériences à travers mon CV !</p>
        <ButtonComp/>
    </div>
</template>

<script>

import TitleComp from './TitleComp.vue'
import ButtonComp from './ButtonComp.vue'

    export default {
        name: "AboutMe",
        components: {
            TitleComp,
            ButtonComp
        },
    }
</script>

<style lang="scss" scoped>
    #about-me {
        text-align: left;        
        
        p {
            font-family: "Poppins", sans-serif;
            font-size: 12px;

            &:last-of-type {
                margin-bottom: 30px;
            }
        }
    }
</style>