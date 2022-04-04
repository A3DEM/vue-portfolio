<template>
    <header>
        <span>AD</span>
        <svg width="25" height="19" viewBox="0 0 25 19" fill="none" xmlns="http://www.w3.org/2000/svg">
            <line x1="25" y1="17.5" x2="-1.31134e-07" y2="17.5" stroke="white" stroke-width="3"/>
            <line x1="25" y1="9.5" x2="-1.31134e-07" y2="9.5" stroke="white" stroke-width="3"/>
            <line x1="25" y1="1.5" x2="-1.31134e-07" y2="1.5" stroke="white" stroke-width="3"/>
        </svg>

    </header>
</template>

<script>
    export default {
        name: "HeaderComp"
    }
</script>

<style lang="scss" scoped>
header {
    
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0px;

    span {
        font-size: 48px;
        font-weight: 800;
        font-style: italic;
    }
}
</style>