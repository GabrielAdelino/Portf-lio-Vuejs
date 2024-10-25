<template>
  <div id="app">
    <Header/>
      <section id="home">
        <h2>Seção1</h2>
        <p>Conteúdo da seção 1.</p>
      </section>

      <section id="about">
        <h2>Seção1</h2>
        <p>Conteúdo da seção 1.</p>
      </section>

      <section id="projects">
        <h2>Seção1</h2>
        <p>Conteúdo da seção 1.</p>
      </section>

      <section id="contact">
        <h2>Seção1</h2>
        <p>Conteúdo da seção 1.</p>
      </section>
  </div>
</template>

<script>
import Header from './components/Header.vue';

export default {
  name: 'App',
  components: {
    Header,
  },
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html {
  scroll-behavior: smooth;
}
/* section {
  margin-top: 500px;    Teste para saber se direcionamento funciona
} */

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
