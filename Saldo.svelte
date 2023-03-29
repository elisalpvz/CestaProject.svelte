

<main>
    <p>{saldo} {resultado}</p>
    <img src={imagen} alt={textoImagen}/>
</main>



<script>

    export let saldo=3
    let resultado
    let imagen
    let textoImagen

    if (saldo > 0) {
        resultado = "Es positivo"
    } else if (saldo < 0) {
        resultado="Es negativo"
    }

    else {
        resultado="Esta todo bien"

    }

</script>