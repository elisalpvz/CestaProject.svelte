
<main>
  <label>
        <span>Nombre</span>
        <input type="text" min="2"  max="20" bind:value={nombre}>
  </label>
  <label> 
       <span>Cuanto pagas?</span>
       <input type="number" bind:value={aPagarCadaUno}>
  </label>
</main>

<script>

import Saldo from "./Saldo.svelte";
    export let aPagarCadaUno
    let pagar
    let nombre
    let aportacion
    let saldo
    $: saldo = aportacion - pagar
    
</script>

<style>


* {
  background-color: rgb(0, 0, 0);
}

</style>











<!--*let usuarios = [
      {
        nombre:"Marco",
        aportacion:"4"
      },

      {
        nombre:"Alvaro",
        aportacion:"6"
      },

      {
        nombre:"Sergio",
        aportacion:"16"
      },
    ]*/


    //console.log(usuarios.length)-->