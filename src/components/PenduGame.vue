<template>
    <div>
      <h1>Jeu du Pendu</h1>
      <form @submit="guess">
        <label for="letter-input">Entrez un mot :</label>
        <input id="letter-input" type="text" v-model="letter" />
        <button type="submit">Devinez</button>
      </form>
        <p>{{ message }}</p>
        <p>Nombre de victoires : {{ correctGuesses }}</p>
        <p>Nombre d'échecs' : {{ incorrectGuesses }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'PenduGame',
    data() {
      return {
        letter: '',
        word: 'hello',
        message: '',
        correctGuesses: 0,
        incorrectGuesses: 0
      }
    },
    methods: {
      guess(event) {
        event.preventDefault()
        console.log(this.letter)
        if (this.word.includes(this.letter)) {
          this.message = 'Mot trouvé.'
          this.correctGuesses++
        } else {
            this.message = 'Mot non trouvé.'
            this.incorrectGuesses++
        }
        if (this.correctGuesses === this.word.length) {
            this.message = 'Vous avez gagné !'
        }
      }
    }
  }
  </script>
  