<template>
    <div class="title">
        <h1>Adem Duran <br> <span>Développeur junior</span></h1>
        <div class="emojis">
            <div class="placeholder"></div>
            <span>+</span>
            <div class="placeholder"></div>
            <span>+</span>
            <div class="placeholder"></div>
        </div>
        <div class="social-links">
            <LinkComp title="LinkedIn"/>
            <LinkComp title="GitHub"/>
            <LinkComp title="Dribbble"/>
            <LinkComp title="Instagram"/>
            <LinkComp title="Email"/>
        </div>
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

    .title {

        .emojis {

            display: flex;
            align-items: center;

            .placeholder {
                height: 40px;
                width: 40px;
                background-color: gray;
            }

            span {
                margin: 0px 12px;
            }
        }

        .social-links {
            margin-top: 20px;
        }
    }
</style>