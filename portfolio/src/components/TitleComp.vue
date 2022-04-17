<template>
    <div class="title">
        <h1>
            Adem Duran <br>
            <span>Développeur junior</span>
        </h1>
        <div class="emojis">
            <img src="@/assets/img/emoji/developer.png" alt="Développeur" width="48" height="48">
            <span>+</span>
            <img src="@/assets/img/emoji/artist.png" alt="Artiste" width="48" height="48">
            <span>+</span>
            <img src="@/assets/img/emoji/ninja.png" alt="Ninja" width="48" height="48">
        </div>
        <div class="social-links">
            <LinkComp link="https://www.linkedin.com/in/adem-duran/" title="LinkedIn"/>
            <LinkComp link="https://github.com/A3DEM/" title="GitHub"/>
            <LinkComp link="https://dribbble.com/a3dem/" title="Dribbble"/>
            <LinkComp link="https://www.instagram.com/a3dem._/" title="Instagram"/>
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
            span {
                margin: 0px 12px;
            }
        }
        .social-links {
            margin-top: 20px;
            display: flex;
            flex-wrap: wrap;
        }
    }

    @media screen and (min-width:1024px) {
        .title {    
            h1 {
                font-size: 48px;
                line-height: 28px;
                margin-top: 55px;
                span {
                    font-size: 24px;
                }
            }
            .emojis {
                font-size: 18px;
                img {
                    width: 60px;
                    height: auto;
                }
            }
            .social-links {
                margin-top: 30px;
            }   
        }
    }
</style>