<template>
  <v-app align="center" >
    <h1>Multiple Counters Component</h1>
      <Counter/>
      
    <h4 > 

<v-btn  v-click=color="blue"> ADD A COUNTER :) </v-btn>
    <transition >
    <p v-show="show">I am rendred only if there is more than one counter...</p>
  </transition>
    
    </h4>
  </v-app>
  
</template>

<script>
import Counter from './components/Counter.vue';


export default {
  name: 'App',

  components: {
  
    Counter,
  },

  data: () => ({
    show: false,
    
    
  }),
};
</script>
