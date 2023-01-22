<script lang="ts" >
    import { defineComponent, ref} from 'vue';
  
    export default {}

  const msg = ref('Dubidu!')
// ref ==> reactive reference
</script>

<template>
<h2>Ciao</h2>
<!-- <p>{{ msg.toLocaleUpperCase() }}</p> -->
<h2> Mmmmm... </h2>
<input ref="input"/>
</template>
