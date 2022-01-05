<template>
    <div id="navbar">
        <div class="hamb" @click="animationToggle = !animationToggle" :class="{change:animationToggle}">
            <div class="bar1"></div>
            <div class="bar2"></div>
            <div class="bar3"></div>
        </div>

        <div class="dropdown" v-show="animationToggle">
            <ul id="first-list">
                <li><a href="#">Products</a></li>
                <li><a href="#">Customers</a></li>
                <li><a href="#">Community</a></li>
                <li><a href="#">Pricing</a></li>
            </ul>
            <ul id="second-list">
                <li><a href="#">Docs</a></li>
                <li><a href="#">Support</a></li>
                <li><a href="#">Login</a></li>
                <li class="button"><a href="#">Sing Up</a></li>
            </ul>
           
        </div>
    </div>
</template>

<script>
export default {
    name: "NavSmart", 
    data() {
        return {
            animationToggle: false,
        }   
    },
}
</script>

<style lang="scss" scoped>
    #navbar {
        .hamb {
            display: inline-block;
            cursor: pointer;
            // float: right;
            .bar1, .bar2, .bar3 {
                width: 35px;
                height: 5px;
                background-color: #333;
                margin: 6px 0;
                transition: 0.4s;
            }
        }

        .change {
            .bar1 {
                -webkit-transform: rotate(-45deg) translate(-9px, 6px);
                transform: rotate(-45deg) translate(-9px, 6px);
            }
            .bar2 {opacity: 0;}

            .bar3 {
                -webkit-transform: rotate(45deg) translate(-8px, -8px);
                transform: rotate(45deg) translate(-8px, -8px);
            }         
        }

        .dropdown {
            position: absolute;
            background-color: #f9f9f9;
            width: 100%;
            left: 0;
            box-shadow: 0 6px 2px -2px balck;
            z-index: 1;
            .first-list {
                margin-top: 20px;
            }
            a {
                text-decoration: none;
                color:black;
            }
            li {
                list-style: none;
            }
            .button {
                margin-top:20px;
                a {
                    color: #2485fd;
                }
            }


        }
    }
                                  
</style>