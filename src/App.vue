<template>
  <div id="app">
    <h3>{{title}}</h3>
    <div class="row">
      <div class="col s1">
        <Character v-for="id in initial_ids" v-bind:id="id"/>

      </div>

    </div>

  </div>
</template>

<script>
import Character from './components/Character'
  export default{
    name:'app',
    data(){
      return{
        title: 'Generate Your Team',
        initial_ids:[1,13,14]
      }
    },
    components:{
      Character
    }
  }
</script>
