
<template>

  <div class="home">
      <h1>Home page</h1>
      <p class="red white--text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quam quo ab veniam, minus, voluptates aliquid delectus est laborum consequuntur molestias dicta accusantium dolorem dolore unde maxime saepe libero repellendus? Iure?</p>
      <p class="pink lightee-4 red--text text--darken-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Itaque, odit repellendus quibusdam eveniet explicabo sequi assumenda natus recusandae, aliquam porro, illo eaque neque architecto! Sapiente, nam laborum? Minima, ea tempora.</p>
      <h1 class="display-4">bigg</h1>
      <h1 class="display-1">bigg</h1>
      <p class="headline">headline</p>
      <p class="subheadline">subheadline</p>
      <v-btn class="pink white--text">click me</v-btn>
       <v-btn flat color="pink">click</v-btn>
      <v-btn dark color="pink" @click="alert=true">eyy</v-btn>
      <v-btn depressed color="pink">hahha</v-btn>
     <v-btn depressed small class="pink white--text">
       <v-icon left>mail</v-icon>
       <span>Email me</span>
     </v-btn>
      <v-btn depressed largue class="pink white--text">
       <v-icon left>mail</v-icon>
       <span>Email me</span>
     </v-btn>
      <v-btn depressed small dark class="purple">
       <v-icon left>mail</v-icon>
       <span>Email me</span>
     </v-btn>
         <v-btn depressed small dark class="purple">
       <v-icon >favorite</v-icon>    
     </v-btn>
      <v-btn class="hidden-md-only">hola</v-btn>
     <v-btn class="hidden-sm-only">hola</v-btn>
     <v-btn class="hidden-md-up">hola</v-btn>
      <v-alert
      v-model="alert"
      dismissible
      type="success">
      This is a success alert that is closable.
    </v-alert>
    <span></span>
</div>
</template>

<script>
/* eslint-disable */
  export default {
   data () {

    return { 
      alert:false

    }
  }, 
  methods:{
    ey:function(){
      return 
    }
  }
  }
</script>
