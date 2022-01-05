<template>
    <div id="navbar">
        <nav>
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
            
        </nav>

    </div>
</template>

<script>
export default {
    name:"NavDesktop",
}
</script>

<style lang="scss" scoped>
    #navbar {

        nav {
            display: flex;
            height: 100%;
            align-items: flex-end;
            #second-list {
                margin-left: 100px;
            }
           

            #first-list, #second-list {
                list-style: none;
                display: flex;

                // margin-bottom: 0;
                a {
                    text-decoration: none;
                    color: black;
                    }
                li {
                    margin: 0px 10px;                 
                }
                .button {
                        a {
                        color: #2485fd;
                    }
                }

            }

        }
       
    }
</style>