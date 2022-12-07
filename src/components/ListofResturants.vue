<template>

    <div >
        <h2>{{Resturant.name}}</h2>
        <div>
            <p>DETAILS</p>
                <ul>
                    <li>id:{{Resturant.id}}</li>
                    <li>cuisinetype:{{Resturant.cuisinetype}}</li>
                    <li>address:{{Resturant.address}}</li>
                    <li>contact:{{Resturant.contact}}</li>
                    <li>DeliveryAvailability:{{Resturant.DeliveryAvailability}}</li>
                </ul>
        </div>
    </div>
</template>

<script>

export default{
    name: 'ListofResturants',
    props:{
        Resturant: Array
    }  
}
</script>

<style scoped>

h2{
    color: #F59924;
    text-align:center;
}

div{
    
    color: #B05626;
    padding: 1em;
    background-color:#101928;
}




</style>
