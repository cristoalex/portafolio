<template>
  <nav>
  </nav>
  <router-view />


  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
  integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">



</template>

<style>
.derchos{
  margin: 20px 0 0; 
  color: #6c757d; 
  font-size: 14px;
}
.bolsa{
  width: 24px; 
  height: 24px; 
  border-radius: 100px;
}
.mani{
  margin-bottom: 20px;
}
.mani a{
  margin-right: 10px;
}
.camaron{
  padding: 20px; 
  text-align:left; 
  border-top: 1px solid #e9ecef; 
  color: antiquewhite; 
  background-color: transparent;
}

nav {
  padding: 30px;
  
}

nav a {
  font-weight: bold;
  font-size: large;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

#app {
  text-align: left;
  padding-left: 30px;
  padding-right: 30px;
  padding-top: 10px;
}
body {
  background-image: url('/src/assets/fondo.jpeg');
  background: linear-gradient(to left, transparent, #09063a),
    url("/src/assets/fondo.jpeg");
  background-size: cover;
  /* Escala la imagen para cubrir el área */
  background-position: center;
  /* Centra la imagen */
  background-repeat: no-repeat;
  
}

.arbol {

  flex-wrap: wrap;
  align-items: center;
}
.mango {

  width: 200px;
  padding: auto; 
  float: right;
}

.gato{
  padding: 2em;
}

.panda {
  padding: 5px;
  text-align: center;
  transition: transform 0.2s ease-in-out;
  color: antiquewhite;
}
.panda img {
  max-width: 100px; 
  height: 100px;
  width: 100px; 
  margin-bottom: 1em;
}


main {
  display: grid;
  grid-gap: 1em;
  padding: 5px;
}
/* Estilos para las cajas individuales */
.box {
  background-color: #eee;
  border-radius: 5px;
  padding: 1em;
}

.box img {
  max-width: 100%;
  height: auto;
}

/* Estilos para las cajas individuales */
.box {
  background-color: #09063a;
  border-radius: 5px;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.3);
  padding: 1em;
  text-align: center;
  transition: transform 0.2s ease-in-out;
}

.box img {
  max-width: 100%;
  height: auto;
  border-radius: 5px;
  margin-bottom: 1em;
}

.box p {
  font-size: 1em;
  font-style: italic;
  color: antiquewhite;
}

.box:hover {
  transform: translateY(-5px);
}

/* Estilos para pantallas más pequeñas */
@media (max-width: 1700px) {

  /* Cambiar a dos columnas */
  main {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, auto);
    gap: 1em;
  }

  .gato{

    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(2, auto);
    gap: 1em;

  }


}

/* Estilos para pantallas más pequeñas */
@media (max-width: 480px) {

  /* Cambiar a una sola columna */
  main {
    display: flex;
    flex-direction: column;
  }
  .gato{
    display: flex;
    flex-direction: column;
  }
    .mango {
      float: none;
      display: block;
      margin: 0 auto 1em;
      max-width: 80%;
    }

  /* Ajustar tamaño de las cajas */
  .box {
    margin-bottom: 1em;
  }
}

.zoomable-image {
  transition: transform 0.5s ease;
}

.zoomable-image:hover {
  transform: scale(1.2);
}

</style>
