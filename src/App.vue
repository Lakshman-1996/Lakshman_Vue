<template>
  <div class="container">
    <MyHeader ResturantName="Top 5 Resturants in USA" Details="List of Resturants" />
    <ResturantDetails :Resturants = "Resturants"/>
    <MyFooter Footer="Please follow us on Socila media" />
    

    

</div>
</template>

<script>

import MyHeader from './components/MyHeader.vue'
import ResturantDetails from './components/ResturantDetails.vue'
import MyFooter from './components/MyFooter.vue'



export default {
  name: 'App',
  components: {    
    MyHeader,
    ResturantDetails,
    MyFooter

  },
  data(){
    return {
      Resturants: [],
      isHidden: false
    }
  },
  methods: {
    // promises

      async fetchResturant(){
         const res= await fetch("http://localhost:7230/Resturants")
         const data= await res.json()
          console.log(data)
         return data
      }
    },
    async created(){
    this.Resturants = await this.fetchResturant()
  }

}

</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');


body {
  font-family: Times New Roman;
  background-color: lightslategray;
}
.container {
  max-width: 400px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 0.3em solid black;
  padding: 30px;
  border-radius: 5px;
  
}

div{
  margin-bottom: 0.5em;
}

</style>
