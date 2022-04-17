<template>
    <a :href="link" target="_blank">{{title}}</a>
</template>

<script>
    export default {
        name: "LinkComp",
        props: {
            link: {
                type: String,
                default: "https://figma.com/" 
            },
            title: {
                type: String,
                default:"Lien"
            }
        }
    }
</script>

<style lang="scss" scoped>
    a {
        color: #0A7AFF;
        text-decoration: none;
        font-size: 12px;
        margin-right: 12px;
    }
    .no-margin {
        margin: 0;
    }
    @media screen and (min-width:1024px) {
        a {
            font-size: 18px;
            margin-right: 18px;
        }
    }
</style>