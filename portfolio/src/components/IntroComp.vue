<template>
    <div id="intro">
        <img src="@/assets/photo-presentation.jpg" alt="Photo de présentation">
        <h1>Adem Duran, <br> Junior Developer</h1>
    </div>
</template>

<script>
    export default {
        name: "IntroComp"
    }
</script>

<style lang="scss" scoped>
#intro {

    display: flex;
    flex-direction: column;
    align-items: center;

    img {
        width: 100%;
        height: auto;
        border-radius: 1000px;
        max-width: 150px;
    }
    h1 {
        font-weight: 800;
        font-style: italic;
        text-transform: uppercase;
        font-size: 48px;
        margin-block-start: 16px;
        margin-block-end: 16px;
        padding-bottom: 16px;
        position: relative;

        &::after {
            content: "";
            background-color: white;
            position: absolute;
            left: 0;
            bottom: 0;
            right: 0;
            height: 3px;
        }
    }
}
</style>