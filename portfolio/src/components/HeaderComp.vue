<template>
    <header>
        <img class="me" src="@/assets/img/photo-presentation-small.webp" alt="C'est moi !" width="110" height="110">

        <div :class="{switch:true, active: isActive }" @click="isActive = !isActive; $emit('toggle')">
            <div class="switch-img">
                <img src="@/assets/img/emoji/sun.png" alt="Light Mode" width="30" height="30">
            </div>
            <div class="switch-item">
                <div class="switch-toggle"></div>
            </div>
            <div class="switch-img">
                <img src="@/assets/img/emoji/moon.png" alt="Dark Mode" width="30" height="30">
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        name:"HeaderComp",
        props: ["mode"],
        data() {
            return {
                isActive: false
            }
        },
        methods: {
            toggle() {
            }
        },
    }
</script>

<style lang="scss" scoped>

    header {

        display: flex;
        flex-direction: column;
        justify-content: flex-start;

        img {
            border-radius: 1000px;
        }

        .switch {
            display: flex;
            align-items: center;
            align-self: flex-start;
            margin-top: 10px;
            
            &-item {
                background-color: #E9E9EB;
                width: 50px;
                height: 30px;
                border-radius: 100px;
                display: flex;
                align-items: center;
                margin: 0px 10px;
            }

            &-toggle {
                background-color: white;
                width: 25px;
                height: 25px;
                border-radius: 100px;
                transform: translateX(4px);
            }
        }

        .active {
            .switch-item {
                background-color: #32D74B;
            }

            .switch-toggle {
                transform: translateX(85%);
            }
        }
    }

    @media screen and (min-width:375px) {
        header {

            flex-direction: row;

            .switch {
                margin-left: auto;
            }
        }
    }
    
    @media screen and (min-width:1024px) {
        header {

            display: inline-flex;
            flex-direction: column;

            .me {
                width: 215px;
                height: auto;
            }
            
            .switch {
                margin-right: auto;
                margin-top: 15px;
            }
        }
    }
</style>