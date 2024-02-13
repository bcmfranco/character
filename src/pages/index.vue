<template>
  <div id="container">


    <div id="character">
      <div id="head"></div>
      <div id="torso">
        <div id="breast"></div>
        <div id="sleeve"></div>
        <div id="hand"></div>
      </div>
      <div id="legs">
        <div class="leg"></div>
        <div class="leg"></div>
      </div>

    </div>

  </div>
</template>

<script>
export default {
  data() {
    return {
      message: "Este es un mensaje dentro del componente."
    };
  },
  methods: {
    changeMessage() {
      this.message = "Nuevo mensaje cambiado por el botón.";
    }
  }
}
</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

*{
  font-family: 'Roboto', sans-serif;
}

#container{
  text-align: center;
}

#container .message {
  color: red;
}

#character{
  border: 3px solid black;
  height: 300px;
  width: 200px;
}

#head{
  border-bottom: 1px solid black;
  height: 100px;
}

#torso{
  border: 3px solid black;
  height: 100px;
  width: 300px;
  display: flex;
  flex-direction: row;
}

#breast{
  height: 100%;
  width: 200px;
}

#sleeve{
  height: 100%;
  width: 50px;
  border-right: 1px solid black;
}

#legs{
  display: flex;
  flex-direction: row;
}

.leg{
  height: 100px;
  width: 100px;
  border-left: 1px solid black;
}

@media only screen and (max-width: 480px) {
  /* Tus estilos específicos para dispositivos móviles aquí */
  #container {
    widows: 400px;
    margin: 0 auto;
  }
}

</style>
