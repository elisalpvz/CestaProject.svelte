
<main>
      <img src="./public/img/encabezado.png" class="logo" alt="Vite Logo" width="300rem" />
      <h1>Calcula las deudas</h1>

      <label>
            <span>Cuantos sois?</span>
            <input type="range" min="2"  max="20" bind:value={cuantos}>
            <p>{cuantos}</p>
      </label>
      <label> 
           <span>Cuanto pagas?</span>
           <input type="number" bind:value={pagar}>
      </label>
      <label>
        <span>Este es tu saldo</span>
        <input type="" bind:value={saldo}>
      </label>
  
<h1>Resultado</h1>
 <Saldo saldo={89}/>
 <Saldo saldo={-30}/>
 <Saldo saldo={0}/>

 <Aportacion aPagarCadaUno={aPagarCadaUno}/>

</main>


<script>
import Saldo from "./assets/Saldo.svelte";
import Aportacion from "./assets/Aportacion.svelte";

      let cuantos = 4;
      let pagar = 25;
      let saldo="3"

      let aPagarCadaUno = (pagar/cuantos);

</script>

<style>

* {
      background-image: url("./public/img/fondo.png");
}

h1 {
      background-color: black;
}
</style>


