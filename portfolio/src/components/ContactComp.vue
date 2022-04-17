<template>
    <div id="contact">
        <h2>Contact</h2>
        <div class="content">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem nulla consectetur recusandae harum quisquam quaerat molestiae ab impedit.</p>
            <LinkComp link="mailto:ademduran6888@gmail.com" title="Envoyer un mail"/>
        </div>
    </div>
</template>

<script>
    import LinkComp from "./LinkComp.vue";
        export default {
        components: { LinkComp }
    }
</script>

<style lang="scss" scoped>
    #contact {
        h2 {
            font-size: 20px;
            margin: 20px 0px 10px 0px;
        }
        p {
            font-size: 12px;
            margin-top: 10px;
            margin-bottom: 10px;
            color: #6D6D6D;
        }
    }
    @media screen and (min-width:1024px) {
        #contact {
            display: grid;
            grid-template-columns: 215px 1fr;
            grid-gap: 50px;
            margin-top: 60px;
            h2 {
                font-size: 30px;
                margin: 0;
            }
            p {
                font-size: 18px;
                margin-top: 0px;
                margin-bottom: 20px;
            }
        }
    }
</style>