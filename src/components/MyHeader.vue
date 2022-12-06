<template>
    <div>
        <h1> {{ResturantName}} </h1>
        <h4> {{Details}} </h4>
    </div>
</template>
    
    <script>
    
    export default{
        name: 'MyHeader',
        props:{
            ResturantName: String,
            Details:String
        }
    }
    
    </script>
    
    <style scoped>
    
    div{
        font-family: Times New Roman Bold;
        text-align: center;
        color: #F59924;
        border: 0.2em solid black;
        padding: 20px;
        border-radius: 2px;
        border-color: #EAE84E;
        background-color:#101928;
        
    }
    
    </style>