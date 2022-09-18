<template>
  <div id="app">
    <main class="content">

      <Board id="first">

        <Card id="task1" draggable="true">
          <p>Card_1</p>
        </Card>

        <Card id="task2" draggable="true">
          <p>Card_2</p>
        </Card>

        <Card id="task3" draggable="true">
          <p>Card_3</p>
        </Card>

      </Board>

      <Board id="second"></Board>

      <Board id="third"></Board>

    </main>
  </div>
</template>

<script>
import Board from './components/dnd-board';
import Card from './components/dnd-card';

export default {
  name: 'App',
  components: {
    Board,
    Card
  }
}
</script>

<style>
   @import './assets/styles/dnd.css'
</style>
