<script>
// JAVASCRIPT

/*
  Come faccio ad utilizzare un componente dentro un altro?
  Si seguono 3 passaggi:
    1)
    2)
    3) Utilizzo del componente
*/
// 1) Importazione
import AppHeader from './components/AppHeader.vue';




// my-component.js
export default {
  data() {
    return { count: 0 };
  },
  // 2) Dichiarazione del componente all'interno dell'oggetto
  components: {
    AppHeader
  }
};
</script>

<template>
 <!-- HTML -->

  <!-- 3) Utilizzo del componente -->
  <AppHeader />

 <div>
    <h2>
        Ciao ragazzi
    </h2>
    <p>
      {{ count }}
    </p>
    <button @click="count++">
      Incrementa count
    </button>
 </div>
</template>

<style scoped>
/* CSS */
</style>
