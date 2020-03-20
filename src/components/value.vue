<template>

<div class="valueExercise">
    <h2>{{headline}}</h2>
    <div class="line"></div>
    <p>{{value}}</p>

    <button @click="increaseValue">Öka</button>
    <button @click="decreaseValue">Minska</button>

    <p class="ownValue">Skriv in din egen siffra</p>
    <div class="inputField">
        <input type="number" placeholder="Skriv en egen siffra" @keyup="handleKeyUp"> 
    </div>
    <button @click="updateValue">Save</button>
    
    <hr>

</div>


</template>

<script>
export default {
  data: () => ({
    headline: "Övningar med Value",
    value:0,
    inputValue:""
  }),
  methods:{
    increaseValue(){
        this.value+=1
    },
    decreaseValue(){
        this.value-=1
    },
    handleKeyUp(event){
        this.inputValue=event.target.value
        console.log("Inputvalue: ", this.inputValue);  
    },
    updateValue(){
        this.value=this.inputValue
    }

  }
};
</script>

<style scoped>
.valueExercise{
    background-color:pink;
    padding:0.5em;
}
.ownValue{
    margin-top:1.5em;
}
h2{

    padding:1em;
}
p{
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
hr{
    background-color:rgb(175, 131, 138);
    padding-left:1em;
    padding-right:1em;
    margin:1em;
}
.line{
    border-top:3px solid rgb(131, 161, 168);
    margin:0 3em 0;
    border-radius:2px
}
.inputField{
   display:flex;
   justify-content:center;
   margin:0.5em;

}



</style>