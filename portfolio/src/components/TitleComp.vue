<template>
    <div class="title">
        <h2>{{title}}</h2>
        <span>{{overlay}}</span>
    </div>
</template>

<script>
    export default {
        name: "TitleComp",
        props: {
            title: {
                type: String,
                default: ""
            },
            overlay: {
                type: String,
                default: ""
            },
        },
    }
</script>

<style lang="scss" scoped>
.title {
    position: relative;
    text-align: center;
 
    h2 {        
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        font-size: 32px;
        font-weight: 800;
        font-style: italic;
        text-transform: uppercase;
        margin-top: 0;
        z-index: 2;
    }
    span {

        font-size: 64px;
        font-weight: 800;
        font-style: italic;
        text-transform: uppercase;
        opacity: 0.1;
    }
}

.mail {
    margin-bottom: 30px;
}
</style>