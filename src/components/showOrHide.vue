<template>
    
    <div class="showHide">
        
    <h2>{{headline}}</h2>
    <div class="line"></div>

    <button @click="displayMsg=true" :disabled="displayMsg">Show</button>
    <button @click="displayMsg=false" :disabled="!displayMsg">Hide</button>
    <div class="displayContainer">
        <p v-show="displayMsg">{{boo}}</p>
    </div>


    </div>

</template>
<script>
export default {
    data: () => ({
       headline:"Show or Hide",
       boo:"Peekabooo",
       displayMsg:false

    })
    
}
</script>

<style scope>
.showHide{
    background-color:rgb(138, 207, 138);
    padding:0.5em;
}
h2{
    padding:0.5em;
}
.line{
    border-top:3px solid rgb(131, 161, 168);
    margin:0 3em 0;
    border-radius:2px;
    padding:1em;
}
button{
    padding:0.5em;
    margin:0.5em;
    border-radius:5px;
    border:none;
    background-color:white;
    box-shadow: 2px 3px 6px rgb(107, 107, 107);
}
p{

    padding:1em;
}
.displayContainer{
    height:2em;
    /* border:1px solid black; */
    margin-bottom:1em;
}

</style>