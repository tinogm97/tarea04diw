<template>
<section id="menu-principal">
    <div id="container">
    <nav>
        <ul>
            <li><a class="elemento_menu" href="#">INICIO</a></li>                       
            <li><a class="elemento_menu" href="#">COMPONENTES</a></li>
            <li><a class="elemento_menu" href="#">PERIFÉRCIOS</a></li>
            <li><a class="elemento_menu" href="#">GAMING</a></li>
            <li><a class="elemento_menu" href="#">PC</a></li>
            <li><a class="elemento_menu" href="#">ACERCA DE</a></li>

        </ul>
    </nav>
    <div id=grupo>
        <button id="registro"> REGISTRO</button>
        <button id="login"> INICIAR SESIÓN</button>
        <span id="icono"><i class="fas fa-shopping-cart"></i></span>
    </div>

</div>
</section>
  
</template>

<script>
export default {

}
</script>

<style scoped>

section#menu-principal {
  
    background: rgb(255, 123, 0);
    
    padding:0.7rem;
}
#container {
    display: flex;
   justify-content: center;
}
ul {
    display:flex;
    list-style: none;
    padding: 0;
   
}
#icono{ 
    color: white;
    margin-left: 3em;
    
}
#grupo{
    margin-left: 5em;
}

.elemento_menu{
    background-color: rgb(255, 123, 0);
    text-decoration: none;
    color:white;
    font-weight: 700;
    padding-left: 1em;
    padding-right: 1em;
}
#registro, #login {
    margin-top: 0.5em;
 background-color:white ;
 color:rgb(255, 123, 0);
    font-weight: 700;
   padding: 0.5em;
 
}




</style>