<template>

    <div class="colormode">

        <h2>{{headline}}</h2>
        <div class="line"></div>

        <div v-bind:class="myNewClass">
            <p>{{chooseColorMode}}</p>
        <button @click="myNewClass='lightmode'">Lightmode</button>
        <button @click="myNewClass='darkmode'">Darkmode</button>
        <p>You have chosen: {{myNewClass}}</p>

        </div>

        
    </div>

    
</template>
<script>
export default {

data: () => ({
headline:"Övning för att byta css class",
myNewClass:"lightmode",
chooseColorMode:"Do you choose the light or the dark path?"
    
})
    
}
</script>
<style scoped>
.colormode{
    background-color:rgb(150, 192, 226);
    padding:1em;
}
.line{
    border-top:3px solid rgb(131, 161, 168);
    margin:0 3em 0;
    border-radius:2px;
    padding:1em;
}
.lightmode{
    /* background-color:rgb(150, 192, 226); */
     background-color:rgb(230, 220, 86);
}
.lightmode >p{
    padding:0.5em;
}

.darkmode{
    background-color:rgb(66, 84, 99);
  
}
.darkmode>button{
    background-color:rgb(151, 132, 142);
    color:white;
}
.darkmode>p{
    color:white;
     padding:0.5em;
 
}

h2{
    padding:0.5em;
}
button{
  
    padding:0.5em;
    margin:0.5em;
    border-radius:5px;
    border:none;
    background-color:white;
    box-shadow: 2px 3px 6px rgb(107, 107, 107);

}

</style>