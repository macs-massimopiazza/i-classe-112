<template>
  <h1 style="color: rgb(97 13 166); font-size: 4rem;">🎡🛝 Vivaaaaa Classe 112 🛝🎡</h1>
  <h3>yayaya</h3>
  <p style="color: #fa1afa">
    💕I vostri insegnanti e coordinatori: Luca, Simone, Giovanni, Massimox2 💕
  </p>
  <h3>Ecco il famoso premio</h3>
  <img src="https://www.coppe-targhe.com/pub/media/catalog/product/cache/1f2776a96cc761aba37519c6315ac844/c/o/coppa-oro-alloro-93176.png" alt="premio">
  <h3 style="color: red;">🦄 Ha vinto lo sport e la passione per la programmazione!11!11!!10!=!=1!=!= 🦥</h3>
  <h3 style="color: #ff0f0f">🥰🤣😱🤧🎍🦖 Qualche parola 🥰🤣😱🤧🎍🦖</h3>
   <h3 style="color: #ff0f0f">uno sviluppatore web è come un cane guida... solo che invece di leccarmi la faccia quando sono triste, mi scrive una canzone in JavaScript.(Alissa e Carmen)</h3>
  <ul>
    <li v-for="(frase, index) in frasi" :key="index">
      {{ frase.testo }}
      <span style="font-style: italic"> -{{ frase.nome }}</span>
    </li>
    <li></li>
  </ul>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      frasi: [
        { testo: "fare il debugging è come essere il detective in un film giallo in cui tu sei anche l'assassino (o forse è stato lo stagista)", nome: "Massimo" },
        { testo: "non è vero, l'assassino è sempre il gatto del maggiordomo", nome: "Massimolaltro" },
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
