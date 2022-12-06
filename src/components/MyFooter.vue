<template>
    <div>
        <h4> {{Footer}} </h4>
    </div>
</template>
    
    <script>
    
    export default{
        name: 'MyFooter',
        props:{
            
            Footer:String
        }
    }
    
    </script>
    
    <style scoped>
    
    div{
        font-family: Times New Roman Regular;
        text-align: center;
        color: #F59924;
        border: 0.2em solid black;
        padding: 20px;
        border-radius: 2px;
        border-color: #EAE84E;
        background-color:#101928;
    }
    
    </style>