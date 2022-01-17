<template>
<Cabecera />
 <div class="container">
  <CaminoMigas />
  <div id="dos-columnas">
    <ProductoImagen />
    <ProductoDatos />
  </div>
  <div class="container">
    <ProductoDescripcion />
    <Especificaciones/>
  </div>
</div>
  <Pie /> 
</template>

<script>
import Cabecera from './components/Cabecera.vue'
import CaminoMigas from './components/CaminoMigas.vue'
import ProductoImagen from './components/ProductoImagen.vue'
import ProductoDatos  from './components/ProductoDatos.vue'
import ProductoDescripcion from './components/ProductoDescripcion.vue'
import Pie from './components/Pie.vue'
import Especificaciones from './components/Especificaciones.vue'


export default {
  name: 'App',
  components: {
    Cabecera,
                CaminoMigas, 
                ProductoImagen, 
                ProductoDatos,
                ProductoDescripcion,
                Especificaciones, 
                Pie
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #002346;
  margin-top: 60px;
}
#dos-columnas{
  display: flex;
  justify-content: center;
  
}
</style>
