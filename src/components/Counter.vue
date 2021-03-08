<template>
    <div id="counter">
<v-app > 
      <v-row  >
      <v-col ><v-btn   @click="addCount"><h3>Click here to increment </h3></v-btn> </v-col>
      <v-col  ><h4 id="cercle">{{ count }}</h4> </v-col>
      </v-row>
      
</v-app>
</div>
</template>


<script>
export default {

  data() {
    
    return {
      count: 0,
    };
  },
  methods: {
    addCount() {
      this.count += 1;
    },
    
   
  }
};
</script>

<style>
#counter {
  height: 45px;
}
#cercle{
   color: white;
    width:40px;
    background:black;
    height:40px;
    text-align:center;
    border-radius:40px;
    line-height: 40px;
    display:inline-bloc;
    
}

</style>