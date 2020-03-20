<template>
  
  <div class="vueIntro">
    <!-- Den här skickas från app.vue -->
    <h3>{{msg}}</h3>

    <!-- <h1 class="welcome">{{welcomeMessage}}</h1>
    
    Ändrar siffror utan funktion
    <p class="number">Utan funktion: {{siffra}}</p>
    <button class="button" @click="siffra+=1">Klicka mig</button> -->

    <!-- Ändrar siffor med funktion -->
       <!-- <p class="number">Med funktion: {{number}}</p>
    <button class="button" @click="addCount()">Addera</button>
    <button class="button" @click="subCount()">Subtrahera</button> -->
    
    <!-- Lägger till egen text -->
    <!-- <div class="inputField">
      <input type="text" @keyup="onKeyUp">
      <p v-if="displayMyText">
        {{ownText}}
      </p> -->
    
    <!-- </div>
    <button class="button" @click="myNewText">Lägg till min nya text</button> -->

    <!-- Ändrar klass/färg  -->
    <!-- <div v-bind:class="myClass">
     <p class="messageFärg">{{message}} </p>
    </div>

    <button class="button" @click="myClass = 'unicorn'">Ljusblå</button>
    <button class="button" @click="myClass = 'racoon'">Magenta</button> -->
  
    <!-- Ändrar text -->
    <!-- <p class="changeText">{{text}}</p>
    <button class="button" @click="changeTextButton()">Ändra texten ovan</button>

  
    <p>Dagens datum: {{date}}</p> -->
  </div>
 
</template>

<script>
export default {
  //allt som ligger i props måste skickas (input output) Se App.vue, det tas emot
  name: 'HelloWorld',
  props: {
    msg: String,
    
  },

  data: () => ({

    welcomeMessage:"Välkommen till Vue Intro!",
    // siffra:13,
    // message:"Klicka för att ändra färg",
    // myClass:"Detta är ett test i myclass",
    // number:0,
    // text:"Ändra mig!",
    // ownText:"",
    // date:new Date(),
    // displayMyText:false
    


  }),
  // methods:{
  //   addCount(){
  //     this.number+=1
  //   },
  //   subCount(){
  //     this.number-=1
  //   },
  //   changeTextButton(){
  //     this.text="Jag har ändrat mig!"
      
  //   },
  //   onKeyUp(event){
  //     this.ownText=event.target.value
  //     console.log("siffra är :", this.ownText);
      
  //   },
  //   myNewText(){
  //     this.displayMyText=true;
  //   }
  
      
    
  // }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

/* .inputField{
  display:flex;
  justify-content:center;
}
.inputField > input{
  padding:0;
  margin:0;
  display:inline-block;

}

.messageFärg{
  margin:0.5em;
}

.unicorn {
	background-color: lightblue;
}
.racoon {
	background-color: rgb(187, 96, 187);
} */
.vueIntro{
  background-color:#42b983;
  padding:0.5em;

  
}
/* .button{
  padding:1em;
  margin:0.5em;
  border:1px solid rgb(83, 109, 117);
  background-color:rgb(107, 139, 151);
  border-radius:0.2em;
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2), 0 6px 20px 0 rgba(0,0,0,0.19);
 
}
.welcome{
  background-color:#CFFE92;
  font-family:-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
 
}
.number{
  background-color:#42b983;
  color:white;
  margin-bottom:0;
  padding:0.5em;
}
.message{
 background-color:#42b983;
 margin-top:1.5em;

}
.changeText{
  padding:0.5em;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
} */

</style>
