<template>
    <header>
        <img src="@/assets/img/photo-presentation-small.jpg" alt="C'est moi !" width="110" height="110">

        <div class="switch">
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
        name:"HeaderComp"
    }
</script>

<style lang="scss" scoped>

    header {

        display: flex;

        img {
            border-radius: 1000px;
        }

        .switch {
            display: flex;
            align-items: center;
            align-self: flex-start;
            margin-left: auto;
            transition: 0.3s ease-in-out;
            
            &-item {
                background-color: #E9E9EB;
                width: 50px;
                height: 30px;
                border-radius: 100px;
                display: flex;
                align-items: center;
                margin: 0px 10px;
                transition: 0.3s ease-in-out;
            }

            &-toggle {
                background-color: white;
                width: 25px;
                height: 25px;
                border-radius: 100px;
                transform: translateX(4px);
                transition: 0.3s ease-in-out;
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
</style>