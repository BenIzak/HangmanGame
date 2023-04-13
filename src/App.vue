<template>
  <img alt="Vue logo" src="https://static.vecteezy.com/system/resources/previews/000/586/123/original/book-reading-logo-and-symbols-template-icons-vector.jpg">
  <PenduGame />
</template>

<script>
import PenduGame from './components/PenduGame.vue';

export default {
  name: 'App',
  components: {
    PenduGame
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
  width: auto;
  height: auto;

  background-color: #f5f5f5;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  row-gap: 20px;
}

#app div {
  width: 100%;
  height: auto;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  row-gap: 20px;
}

#app form {
  width: 100%;
  height: auto;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  row-gap: 20px;

  background-color: #fff;
  border-radius: 10px;
  padding: 20px;
}

#app form label {
  width: 100%;

  text-align: center;
  font-size: 1.2rem;

  font-weight: bold;
}

#app form input {
  width: 100%;
  height: 50px;

  border: none;
  border-radius: 10px;
  padding: 0 20px;
  font-size: 1.2rem;

  background-color: #f5f5f5;
}

#app form input:focus {
  outline: none;
}

#app form button {
  width: 100%;
  height: 50px;

  border: none;
  border-radius: 10px;
  padding: 0 20px;
  font-size: 1.2rem;

  background-color: #42b983;
  color: #fff;
}

#app form button:focus {
  outline: none;
}

#app form button:hover {
  cursor: pointer;

  background-color: #3da777;
}

img {
  width: 150px;
  height: 150px;

  border-radius: 50%;
}

h1, h2 {
  font-weight: bold;
}

p {
  font-size: 1.2rem;
}

body {
  width: 100%;
  min-width: 320px;
  
  height: 100vh;

  background-color: #f5f5f5;

  display: flex;
  justify-content: center;
  align-items: center;

}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

</style>
