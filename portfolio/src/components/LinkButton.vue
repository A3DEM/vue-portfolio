<template>
    <a :href="link">
        {{text}}
    </a>
</template>

<script>
    export default {
        name: "LinkButton",
        props: {
            link: {
                type: String,
                default: "https://www.ademduran.fr"
            },
            text: {
                type: String,
                default: "Découvrir le projet"
            }
        },
    }
</script>

<style lang="scss" scoped>
    a {
        background-color: #BC8F53;
        color: white;
        border: none;
        font-family: dharma-gothic-m, sans-serif;
        text-transform: uppercase;
        text-decoration: none;
        font-size: 20px;
        font-style: italic;
        font-weight: bold;
        padding: 10px 20px;
        margin-bottom: 20px;
    }

</style>