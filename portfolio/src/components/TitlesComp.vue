<template>
    <div class="titles">
        <div v-for="item in items" v-bind:key="item"  class="titles-container">
            <div class="titles-title">
            <h2>{{item.title}}</h2>
            <div class="placeholder"></div>
            </div>
            <p>{{item.paragraph}}</p>
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
                        title:"Propulsé par la créativité",
                        paragraph:"Chaque projet est l'opportunité de laisser parler son imagination. Découvrez la mienne au travers de mes projets !",
                    },
                    {
                        title:"Guidé par le développement web",
                        paragraph:"Au cœur de ma formation, le développement web est le terrain sur lequel je peux m'exprimer. Surtout lors de projets créatifs.",
                    },
                    {
                        title:"Passionné par le football",
                        paragraph:"L'esprit d'équipe, la détermination et la rigueur sont quelques unes de mes qualités qui découlent de mon amour du football.",
                    }
                ]
            }
        },
    }
</script>

<style lang="scss" scoped>
.titles {

    margin-top: 40px;

    &-container {
        text-align: left;
        position: relative;
        margin-bottom: 40px;

        h2 {
            font-size: 16px;
            margin: 0;
        }
        p {
            font-size: 12px;
            margin-top: 5px;
            margin-bottom: 0;
            color: #6D6D6D;
        }
        .placeholder {
            height: 20px;
            width: 20px;
            background-color: gray;
            margin-left: 10px;
        }
    }

    &-title {
        display: flex;
    }

    
}
</style>