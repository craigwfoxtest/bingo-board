<template>
  <div id="app">
    <h1>Bingo Board</h1>
    <BingoBoard />
    <WinnerTable />
  </div>
</template>

<script>
import BingoBoard from './components/BingoBoard.vue'
import WinnerTable from './components/WinnerTable.vue'

export default {
  name: 'app',
  components: {
    BingoBoard,
    WinnerTable
  }
}
</script>

<style>
:root {
  --ffcond: 'Oswald', sans-serif;
  --ffbase: 'Roboto', sans-serif;
}
html {
  margin: 0;

  font-size: 10px;
  font-family: var(--ffbase);
}

body {
  margin: 0;
  padding: 2rem;

  font-size: 1.8rem;
}

#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  text-align: center;
}

h1, h2, h3, h4, h5, h6 {
  font-family: var(--ffcond);
}
</style>
