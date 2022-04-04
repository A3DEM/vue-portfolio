<template>
    <div id="contact-me">
        <TitleComp class="mail" title="Contact" overlay="Restons en contact"/>

        <LinkButton link="mailto:contact@ademduran.fr" text="Me contacter"/>
    </div>
</template>

<script>
    import TitleComp from "./TitleComp.vue";
    import LinkButton from "./LinkButton.vue";
    export default {
        name: "ContactMe",
        components: { TitleComp, LinkButton }
    }
</script>

<style lang="scss" scoped>
    #contact-me {
        padding-bottom: 20px;
        margin: 35px 0px 20px 0px;

    }
</style>