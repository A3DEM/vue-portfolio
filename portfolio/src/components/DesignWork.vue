<template>
    <div id="design">
        <h2>Projets graphisme</h2>
        <ProjectComp type="design"/>
    </div>
</template>

<script>
    import ProjectComp from "./ProjectComp.vue"
    export default {
        name:"DesignWork",
        components: {
            ProjectComp,
        },
    }
</script>

<style lang="scss" scoped>
    #design {
        h2 {
            font-size: 20px;
            margin: 20px 0px 10px 0px;
        }
    }
    @media screen and (min-width:1024px) {
        #design {
            display: grid;
            grid-template-columns: 215px 1fr;
            grid-gap: 50px;
            margin-top: 60px;
            h2 {
                margin: 0px;
                font-size: 30px;
            }
        }
    }
</style>