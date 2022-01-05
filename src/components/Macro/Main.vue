<template>
  <div id="main">
       
      <!-- Jumbotron  -->
      <Jumbotron/>

      <!-- sections -->
      <Section1/>
      <Section2/>
      <Section3/>
      <Section4/>
      <Section5/>
      <Section6/>
      <Section7/>
  </div>
</template>

<script>
import data from "../../share/data"
import Section1 from "../Sections/Section1.vue"
import Section2 from "../Sections/Section2.vue"
import Section3 from "../Sections/Section3.vue"
import Section4 from "../Sections/Section4.vue"
import Section5 from "../Sections/Section5.vue"
import Section6 from "../Sections/Section6.vue"
import Section7 from "../Sections/Section7.vue"
import Jumbotron from "../Sections/Jumbotron.vue"


export default {
    name:"Main",
    components: {
        Jumbotron,
        Section1,
        Section2,
        Section3,
        Section4,
        Section5,
        Section6,
        Section7,

    },
    data() {
        return {
            data
        }
    }
}
</script>

<style lang="scss" scoped>
    #main {
        padding-top: 80px ;
    }
</style>