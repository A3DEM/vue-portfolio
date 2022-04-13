<template>
    <footer>
        Made with <div class="placeholder"></div> + <div class="placeholder"></div> in Mulhouse, France.
    </footer>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
    footer {
        font-size: 14px;
        display: flex;
        align-items: center;
        margin-top: 30px;

        .placeholder {
            height: 15px;
            width: 15px;
            background-color: gray;
            margin: 0px 5px;
        }
    }
</style>