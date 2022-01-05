<template>
    <div id="header">

            <!-- Header Bar  -->
            <div class="container container-lg">
                <div class="img">
                    <img  src="../../assets/img/logo.png" alt="digital-ocean-logo">
                </div>
                <NavDesktop v-if="screen > 960"/>
                <NavSmart v-else />
            </div>
           
    </div>
</template>

<script>
import data from "../../share/data";
import NavDesktop from "../Sections/NavDesktop.vue"
import NavSmart from "../Sections/NavSmart.vue"
export default {    
    name: "Header",
    components: {
        NavDesktop, 
        NavSmart,
    },
    data() {
        return {
            data,
            screen: window.innerWidth,
            menu: []
        }
    },

}
</script>

<style lang="scss" scoped>
    
    #header {
        width: 100%;
        border-bottom: 1px solid black;
        position: fixed;
        height: 80px;
        background-color: white;
        .container {
            // height: 100px;
            padding: 15px 10px;
            // width: 1140px;
            margin: auto;
            display: flex;
            justify-content: space-between;
            .img {
                height: 100%;
                width: 30%;
                align-self: center;
                img  {
                    width: 70%;
}
            }
        }
    }

</style>






