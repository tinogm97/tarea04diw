<template>
  <section id="producto-descripcion">
      <h1>DESCRIPCIÓN DEL PRODUCTO</h1>
      <div id="descripcion">
            <p>Entra en la nueva generación de procesadores AMD Ryzen 5 con el nuevo PCCOM Silver. Su procesador AMD Ryzen 5 3600 de seis núcleos, 
            16 GB de RAM DDR4 y su potente tarjeta gráfica RTX3060 te ofrecerán toda la potencia necesaria para disfrutar de los últimos juegos del mercado.</p>

            <p>Disfruta de la mejor tecnología Nvidia en tus juegos favoritos, con la gráfica serie RTX incluida en este increíble PC:</p>
            <ul>
            <li> <span>Arquitectura NVIDIA Ampere:</span> La nueva arquitectura NVIDIA Ampere ofrece el juego definitivo y presenta los núcleos avanzados de trazado de rayos de segunda generación 
            y los Tensor Cores de tercera generación con un rendimiento superior. </li>
            
            <li><span>Aceleración IA de DLSS:</span>  NVIDIA DLSS es una renderización de IA revolucionaria que aumenta 
            las velocidades de fotogramas con una calidad de imagen sin concesiones utilizando Tensor Cores de procesamiento de IA dedicados en GeForce RTX. 
            Dispondrás de margen de rendimiento para establecer los ajustes y las resoluciones necesarias a fin de disfrutar de una experiencia visual increíble. 
            La revolución de la IA ha llegado al gaming.</li>

            <li><span>La victoria se mide en milisegundos:</span> NVIDIA Reflex ofrece la máxima ventaja competitiva. La latencia más baja. La mejor capacidad de respuesta. 
            Gracias a las GPU GeForce RTX serie 30 y los monitores NVIDIA G-SYNC.</li>
            </ul>
            <h3>Vídeos / Reseñas</h3>
            <div id="video">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/ncapm2q5Seo?controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
      </div>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>
h1{
    text-align: left;
    margin: 0 3em;
}
#producto-descripcion {
    margin:3em 7em;
}
span{
    font-weight: bold;
}
li{
    margin: 1em 0;
}
#producto-descripcion h1 {
    color: rgb(240, 120, 9);
    font-size: 1.5em;
}
#descripcion{
    text-align: justify;
    margin: 2em 8em;
    
}
#descripcion div{
    display: flex;
    justify-content: center;
}
h3{
    margin-top: 2em;
    text-align: left;
       color: rgb(240, 120, 9);
}
#video{
    margin-top: 2em;
    margin-left: -45em;
}

</style>