<template>
  <div id="app">
    <h1 style="color: rgb(97 13 166); font-size: 4rem;">🎡🛝 Vivaaaaa Classe 112 🛝🎡</h1>
    <h3>yayaya</h3>
    <p style="color: #fa1afa">
      💕I vostri insegnanti e coordinatori: Luca, Simone, Giovanni, Massimox2 💕
    </p>
    <h3>Ecco il famoso premio sudato con tanta fatica</h3>
    <img src="https://www.coppe-targhe.com/pub/media/catalog/product/cache/1f2776a96cc761aba37519c6315ac844/c/o/coppa-oro-alloro-93176.png" alt="premio">
    <h3 style="color: red;">🦄 Ha vinto lo sport e la passione per la programmazione!11!11!!10!=!=1!=!= 🦥</h3>
    <h3 style="color: #ff0f0f">🥰🤣😱🤧🎍🦖 Qualche parola 🥰🤣😱🤧🎍🦖</h3>
    <ul>
      <li v-for="(frase, index) in frasi" :key="index">
        {{ frase.testo }}
        <span style="font-style: italic"> -{{ frase.nome }}</span>
      </li>
    </ul>
    <span class="heart" :class="{ 'clicked': loveClicked }" @click="toggleLove">&#10084;</span>
    <p>Made with &#10084; by myself. Don't waste your money! Cit. Cosimo</p>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      frasi: [
        { testo: Forza Milan, nome: Matteo},
        { testo: "fare il debugging è come essere il detective in un film giallo in cui tu sei anche l'assassino (o forse è stato lo stagista)", nome: "Massimo" },
        { testo: "non è vero, l'assassino è sempre il gatto del maggiordomo", nome: "Massimolaltro" },
        { testo: "Proof of Steak is love, Proof of Steak is life UwU", nome: "Fonta" },
        { testo: "Ma precisamente, questo <s>Kafkian</s> Boolean, chi è?", nome: "Ale R" },
        { testo: "hello world from murderer!", nome: "Gianluca" },
        { testo: "E se la vita fosse solo un loop infinito, con il debug come unico modo per trovare la felicità?", nome: "Domenico"},
        { testo: "ero ateo fino a quando non ho scoperto che ero un Dio nel mondo di LoL. 🤡", nome: "aChuckArell" },
        { testo: "essere dei chad ", nome: "CHAD" },
        { testo: "Perchè nonostante una chiave USB ha due facce, riesco sempre ad inserirla al terzo tentativo?", nome: "Alessio" },
        { testo: "Finalmente le lezioni sono finite!!!", nome: "Francesco" },
        { testo: "Quando una cosa ti va male, rifalla 21 volte", nome: 'Cristopher'},
      ],
      loveClicked: false
    };
  },
  methods: {
    toggleLove() {
      this.loveClicked = !this.loveClicked;
    }
  }
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

.heart {
  cursor: pointer;
}

.clicked {
  color: red;
}
</style>
