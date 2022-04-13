<template>
    <div id="design">
        <h2>Projets graphisme</h2>
        <DesignProjectComp/>
    </div>
</template>

<script>
import DesignProjectComp from "./DesignProjectComp.vue"
    export default {
        name:"DesignWork",
        components: {
            DesignProjectComp,
        },
    }
</script>

<style lang="scss" scoped>
    #design {
        h2 {
            margin: 20px 0px 10px 0px;
        }
    }
</style>