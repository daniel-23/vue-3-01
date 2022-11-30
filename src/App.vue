<script>
export default {
  data: () => ({
    contador: 0,
  }),
  methods: {
    suma() {
      this.contador++;
    },
    resta() {
      if (this.contador > 0) {
        this.contador--;
      }
    },
    reset() {
      this.contador = 0;
    },
  },
};
</script>

<template>
  <img src="./assets/logo.svg" alt="Logo" />
  <h1>Hola mundo desde vue js 3</h1>
  <hr />
  <p>Contador: {{ contador }}</p>

  <button v-on:click="suma">+1</button>
  <button @click="resta">-1</button>
  <button @click="reset">Reset</button>
</template>

<style scoped>
h1 {
  background-color: bisque;
}
</style>
