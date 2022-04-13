<template>
    <div id="web">
        <h2>Projets web</h2>
        <WebProjectComp/>
    </div>
</template>

<script>
import WebProjectComp from "./WebProjectComp.vue"
    export default {
        name:"WebWork",
        components: {
            WebProjectComp,
        },
    }
</script>

<style lang="scss" scoped>
    #web {
        h2 {
            margin: 20px 0px 10px 0px;
        }
    }
</style>