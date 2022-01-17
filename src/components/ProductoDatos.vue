<template>
  <section id="producto-datos">
      <h1>PC montado Silver AMD Ryzen 5 3600<br>16GB/480GBSSD+1TB/RTX3060</h1>
      <h2>1383,22€</h2>
      <div id="wrapper">
          <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
          <input id="cantidad" type="text" name="name" :value="contador">
          <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
      </div>
      <div >
        <p id="so">Instalación del Sistema Operativo: ( 60€ )<input type="checkbox" id="check" @change="visible()" /><br></p>
        <select class="oculto" >
          <option value="win10">Windows 10</option>
          <option value="win11">Windows 11</option>
          <option value="lin">Linux</option>
        </select> 
      </div>
      <br>
      <div id="botones">
      <button id="boton"> AÑADIR AL CARRITO</button><button id="comprar"> COMPRAR</button></div>
  </section>
</template>

<script>
export default {
  Name: 'ProductoDatos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        },
        visible(){
          let check=document.querySelector("#check");
          if(check.checked){
            document.querySelector("select").style.display="block"
            let h2=document.querySelector("h2")
            h2.innerHTML="1443,22€"
           
          }else {
            document.querySelector("select").style.display='none';

            let h2=document.querySelector("h2")
            h2.innerHTML="1383,22€"
            
            
          }
        }
    }


}
</script>

<style scoped>
.oculto{
  display: none;
}
#so{
  margin: 1em 0;
}
#sin-iva{
  font-size: 0.5em;
  color: rgb(1, 0, 36);
  font-weight: 300;
  margin-left: 1em;
}

section#producto-datos {
 display: flex;
 flex-direction: column;
 align-items: center;
 justify-content: center;
 margin-top: -10em;
 margin-left: 5em;
}
h1 {
  color: rgb(3, 0, 34);
  font-size: 1.5em;
}
h2 {
  font-size:1.7rem;
  color: rgb(255, 123, 0);
}

#wrapper {
  height: 2em;
  display: flex;
}

#cantidad {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  border: 1px solid #d8d8d8;
}
.btn {
  border: 1px solid #d8d8d8;
  width: 1.8rem;
}
button:focus, input:focus {
  outline: 0;
}
#botones{
  display: flex;
}
#boton{
margin-top: 2em;
padding: 0.7em;
font-size: 1em;
background-color: rgb(255, 123, 0);
color: white;
font-weight: bold;
margin-right: 0.5em;
}
#comprar{
  margin-top: 2em;
padding: 0.7em;
font-size: 1em;
background-color: white;
color: rgb(255, 123, 0);
font-weight: bold;
margin-left: 0.5em;
}
#boton:hover{

background-color: white;
color: rgb(255, 123, 0);
border-color: rgb(255, 123, 0);

}
#comprar:hover{

background-color: rgb(255, 123, 0);
color: white;
border-color: white;
}
select{
  
padding: 0.7em;

background-color: white;
color: rgb(255, 123, 0);
font-weight: bold;
margin-left: 0.5em;
font-size: 1em;
}
</style>