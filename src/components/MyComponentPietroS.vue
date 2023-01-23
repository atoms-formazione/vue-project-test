<script lang="ts" >
    // import { defineComponent, ref} from 'vue';
  
    export default {
      name: "PietroS",
      props: ['name']
    }

  // const msg = ref('Dubidu!')
// ref ==> reactive reference
</script>

<template>
<h2 class="ciao">Ciao {{ name }}</h2> 
<!-- <p>{{ msg.toLocaleUpperCase() }}</p> -->
</template>

<style>
.ciao{
color: cadetblue;
border: 1px white solid;
padding: 10px;
margin: auto;
}
</style>