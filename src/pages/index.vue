<template>
  <div id="container">


    <div id="character">
      <div id="top" class="skin_1"></div>
      <div id="medium">
        <div id="breast" class="shirt_tecnopink"></div>
        <div id="sleeve" class="shirt_tecnopink"></div>
        <div id="hand" class="skin_1"></div>
      </div>
      <div id="bottom">
        <div id="short" class="gray_short"></div>
        <div id="legs">
          <div class="leg skin_1"></div>
          <div class="leg skin_1"></div>
        </div>
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

#top{
  border-bottom: 1px solid black;
  height: 100px;
}

#medium{
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

#hand{
  width: 50px;
}

#sleeve{
  height: 100%;
  width: 50px;
  border-right: 1px solid black;
}

#bottom{
  display: flex;
  flex-direction: column;
}

#short{
  width: 100%;
  height: 50px;
  border-bottom: 1px solid black;
}

#legs{
  display: flex;
  flex-direction: row;
}

.leg{
  height: 50px;
  width: 100px;
  border-left: 1px solid black;
  border-bottom: 3px solid black;
}

.blue_shirt{
  background-color: rgb(60, 75, 109);
}

.gray_short{
  background-color: lightgray;
}

.skin_1{
  background-color: #ffdbac;
}

.shirt_tecnopink{
  background: rgb(63,94,251);
  background: radial-gradient(circle, rgba(63,94,251,1) 0%, rgba(252,70,107,1) 100%);
}

@media only screen and (max-width: 480px) {
  /* Tus estilos específicos para dispositivos móviles aquí */
  #container {
    widows: 400px;
    margin: 0 auto;
  }
}

</style>
