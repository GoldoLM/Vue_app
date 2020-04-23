<template>
  <div>  
    <h1>{{ title + i+ times}}</h1>
    <button @click="iAmClicked()">Click me!</button>
    <button @click="resetInc()">Reset !</button>
  </div>
</template>
 
<script>
    export default {
       
        data() {
            return {
                title: 'you have cliked : ',
                i : 0 ,
                times :" times",
            }
        },
        methods: {

             resetInc(){
                 this.title=" you have cliked : "; 
                 this.i = 0 ;
                 this.times =" times";
            },
        
            iAmClicked() {
                this.i +=1;
                this.title = "you have cliked : ";
                this.times =" times";
            },

           
        }
    };
</script>