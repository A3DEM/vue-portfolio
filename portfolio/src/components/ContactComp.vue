<template>
    <div id="contact">
        <h2>Contact</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Autem nulla consectetur recusandae harum quisquam quaerat molestiae ab impedit.</p>
        <LinkComp link="mailto:ademduran6888@gmail.com" title="Envoyer un mail"/>
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
            margin: 20px 0px 10px 0px;
        }
        p {
            font-size: 12px;
            margin-top: 10px;
            margin-bottom: 10px;
            color: #6D6D6D;
        }
    }
</style>