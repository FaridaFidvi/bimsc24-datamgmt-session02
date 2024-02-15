<!-- the script is where the js code goes -->
<script setup>
import { ref } from "vue" // you need this to use ref()

//Ner reference variable
let user = ref("Farida")
let computername = ref("Dendron")

//define function
function say(message) {
  alert(message)
}


</script>





<!-- the template is where the html code goes -->
<template>
 <div id="navbar" class="container">  
        <div id="title">Testing Computer Skills of {{ computername }}</div>
       
    </div>

    <div id="flex">

        <div id="sidebar" class="container"> Greeting you
            

            <div><button @click="say('hello')">Hola</button></div>
        </div>

        <div id="main" class="container"> Bidding Farewell
            
           <div> <button @click="say('bye')">Adios</button></div>

        </div>
   
   
   
    </div>



</template>



<!-- style is where the css code goes -->
<style scoped>

html{
    
    background-color: rgb(59, 59, 59); 
    color: white;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

body{

    margin:0;
}

div{

    /* put the borders in the inside of container */
    box-sizing: border-box;
}

#navbar{

    height: 50px;
    border-color: red;
background-color: palevioletred;

}

#flex{
    
    display: flex;
    height: calc(100vh - 50px);
}

#sidebar{
    
    width:20%;
    border-color: blue;
background-color: white;
color: black;
}

#main{
    width:80%;
    border-color: green;
background-color: lightblue


}

#title{
    width: 70%;
    float:left;
}

.container{

    border-style: dotted;
    border-width: 1px;

}
</style>