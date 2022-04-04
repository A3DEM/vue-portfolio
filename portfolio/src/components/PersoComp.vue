<template>
    <div class="about-comp">
        <div v-for="item in items" v-bind:key="item"  class="about-comp-parent">
            <h2>{{item.title}}</h2>
            <p>{{item.paragraph}}</p>
            <img :src="require(`@/assets/svg/${item.filename}`)" :alt="item.alt">
        </div>
    </div>
</template>

<script>
    export default {
        name:"PersoComp",
        data() {
            return {
                items: [
                        {
                        title:"propulsé par la créativité",
                        paragraph:"Chaque projet est l'opportunité de laisser parler son imagination. Je vous propose de la découvrir au travers de mes projets. ",
                        filename:"rocket.svg",
                        alt:"Fusée"
                    },
                    {
                        title:"Guidé par le dev. web",
                        paragraph:"Au cœur de ma formation, le développement web est le terrain sur lequel je peux m'exprimer. Surtout lors de projets créatifs.",
                        filename:"dev.svg",
                        alt:"Développement web"
                    },
                    {
                        title:"Passionné par le football",
                        paragraph:"L'esprit d'équipe, la détermination et la rigueur sont quelques unes de mes qualités qui découlent de mon amour du ballon rond.",
                        filename:"football.svg",
                        alt:"Football"
                    }
                ]
            }
        },
    }
</script>

<style lang="scss" scoped>
.about-comp-parent {

    text-align: left;
    position: relative;

    h2 {
        text-transform: uppercase;
        font-size: 32px;
        font-style: italic;
        padding-bottom: 9px;
        position: relative;

        &::after {
            content: "";
            background-color: white;
            position: absolute;
            left: 0;
            bottom: 0;
            right: 0;
            height: 3px;
            max-width: 50px;
        }
    }
    p {
        font-family: poppins, sans-serif;
        font-size: 12px;
        margin-block-start: 12px;
        margin-block-end: 12px;
    }

    img {
        position: absolute;
        top: 0;
        right: 0;
        width: 25px;
        height: auto;
        margin-top: 2px;
    }
}
</style>