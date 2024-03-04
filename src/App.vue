<template>
  <h1 style="color: rgb(97 13 166); font-size: 4rem;">🎡🛝 Vivaaaaa Classe 112 🛝🎡</h1>
  <h3>yayaya</h3>
  <p style="color: #fa1afa">
    💕I vostri insegnanti e coordinatori: Luca, Simone, Giovanni, Massimox2 💕
  </p>
  <h3 style="color: #ff0f0f">🥰🤣😱🤧🎍🦖 Qualche parola 🥰🤣😱🤧🎍🦖</h3>
  <ul>
    <li v-for="(frase, index) in frasi" :key="index">
      {{ frase.testo }}
      <span style="font-style: italic"> -{{ frase.nome }}</span>
    </li>
    <li><img src="https://www.zooplus.it/magazine/wp-content/uploads/2020/10/1-37-768x512.jpg" alt="gattino"></li>
  </ul>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      frasi: [
        { testo: "fare il debugging è come essere il detective in un film giallo in cui tu sei anche l'assassino (o forse è stato lo stagista)", nome: "Massimo" },
      ],
    };
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

body {
  background-color: #fbdca4;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1a6a00;
}

img {
  width: 400px;
}

li {
  font-size: 20px;
  margin-bottom: 5px;
}

h1,
h3,
p,
ul {
  margin-bottom: 20px;
}

.proj {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
