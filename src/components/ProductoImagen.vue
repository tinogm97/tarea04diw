<template>
  <section id="producto-imagen">
      <div > 
          <img id="foto-principal" v-bind:src="fotos[0]" alt="PC montado Silver AMD Ryzen 5" copyright="cc-by Pccomponentes">
      </div>
        <div id="mini">
          <a class="img-mini" @click="cambiarFoto(1)"><img  v-bind:src="fotos[1]" alt="PC montado Silver AMD Ryzen 5" copyright="cc-by Pccomponentes"></a>
          <a class="img-mini" @click="cambiarFoto(2)"><img  v-bind:src="fotos[2]" alt="PC montado Silver AMD Ryzen 5" copyright="cc-by Pccomponentes"></a>
          <a class="img-mini" @click="cambiarFoto(3)"><img  v-bind:src="fotos[3]" alt="PC montado Silver AMD Ryzen 5" copyright="cc-by Pccomponentes"></a>
          <a class="img-mini" @click="cambiarFoto(4)"><img  v-bind:src="fotos[4]" alt="PC montado Silver AMD Ryzen 5" copyright="cc-by Pccomponentes"></a>
          <a class="img-mini" @click="cambiarFoto(5)"><img  v-bind:src="fotos[5]" alt="PC montado Silver AMD Ryzen 5" copyright="cc-by Pccomponentes"></a>
          
        </div>
      </section> 
      
</template>

<script>
export default {
    Name: 'ProductoImagen',
    data () {
        return {
            fotos: [
                require ('../assets/e1.jpg'),
                require ('../assets/e1.jpg'),
                require ('../assets/e2.jpg'),
                require ('../assets/e3.jpg'),
                require ('../assets/e4.jpg'),
                require ('../assets/e5.jpg')]
        }
    },
    methods: {
        cambiarFoto(id) {
            this.fotos[0] = this.fotos[id]
        }
    }

}
</script>

<style scoped>

#producto-imagen {
    border-radius: 25px;
    padding: 1rem;
    margin-top: 2em;
    margin-right: 5em;
    
    
}
.img-mini {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
}
.img-mini img {
    width: 100px;
    border:1px solid #3f260552;
    
}
#mini{
    display: flex;
    justify-content: center;
    margin-top: 2em;
}
#foto-principal{
    margin-top: -2em;
}
</style>