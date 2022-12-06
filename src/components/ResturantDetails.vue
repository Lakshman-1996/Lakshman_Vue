<template>
    <div class="ResturantDetails">
        <div v-for="Resturant in Resturants" :key="Resturant.id" >     
               <ListofResturants :Resturant="Resturant"/>
        </div>
    </div>

</template>

<script>
import ListofResturants from './ListofResturants.vue'
export default {
    name: 'ResturantDetails',
    components: {
        ListofResturants
    },
    props:{
        Resturants: Array

    }
}


</script>


<style>
.ResturantDetails{

    font-family: Times New Roman Bold;
    border: 0.2em solid black;
    border-radius: 2px;
    border-color: #EAE84E;
}

</style>