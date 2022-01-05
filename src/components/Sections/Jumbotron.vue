<template>
  <div id="jumbotron" >
      <div class="container-lg">
          <div class="row">
            <div class=" left-col col-12 col-md-8  ">
                <h2>The simplest cloud platform for developers 	&amp; teams</h2>
                <p>Deploy, manage, and scale cloud applications faster and more efficiently on DigitalOcean. We make managing infrastructure easy for teams and businesses, whether you're running one virtual machine or ten thousand.</p>
            </div>
            <div class=" right-col col-12 col-md-4 ">
                <h3>Deploy your app in seconds.</h3>
                <h3>Get started now.</h3>
                <input type="text" placeholder="Email">
                <input type="text" placeholder="Password">
                <div class="button-create">Create your acccount</div>
                <div class="button-g">
                    <img src="../../assets/img/google-icon.png" alt="">
                    Sign up with Google</div>
                <p>By signin up you agree to the <a href="#">Terms of service</a></p>
            </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"Jumbotron",
}
</script>

<style lang="scss" scoped>
    #jumbotron {
        background-image: url("../../assets/img/bg-banner-home.jpg") ;
        padding: 45px 10px;

        .left-col {
            color:white;
            h2 {
                font-weight: bold;
                font-size: 30px;
            }
            p {
                font-size: 20px;
                margin-bottom: 8px;
            }

            @media (min-width: 577px) {
                h2 {
                    font-size: 40px;
                }   
            }
            @media (min-width: 1140px) {
                h2 {
                    font-size: 50px;
                }   
            }
        }
        .right-col {
            background-color: white;
            padding: 30px 25px;
            border-radius: 5px;

            h3 {
                text-align: center;
                font-weight: bold;

            }
            h3:nth-child(2) {
                color:#2485fd;
            }

            input {
                width: 100%;
                border: none;
                margin: 10px 0px;
                font-size: 13px;
                font-weight: bold;
            }

            .button-create, .button-g {
                width: 100%;
                margin: 8px 0px;
                font-size: 12px;
                text-align: center;
                font-weight: bold;
            }
            .button-create {
                background-color: #2485fd;
                padding: 4px;
                color: white;
                border-radius: 5px;
            }
            .button-g img{
                width: 15px;
                float: left;
            }
            p {
                font-size: 11px;
                text-align: center;
                margin-bottom: 0;
            }
        }
    }
</style>