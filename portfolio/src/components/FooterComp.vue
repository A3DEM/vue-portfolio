<template>
    <footer>
       Copyright © 2021 Adem Duran. <br> Made with ❤️ + <img src="@/assets/svg/vuejs.svg" alt="Vue JS"> in Mulhouse, FRANCE.
    </footer>
</template>

<script>
    export default {
        name: "FooterComp"
    }
</script>

<style lang="scss" scoped>
    footer {
        background-color: #1e1e1e;
        font-family: poppins, sans-serif;
        padding: 20px 50px;
        text-transform: uppercase;
        font-weight: bold;
        font-size: 14px;

        img {
            width: 14px;
            height: auto;
            transform: translateY(10%);
            margin: 0px 3px;
        }
    }
</style>