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
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body{
    background-color: #D0D0C0;
  }

  .content{
    display: flex;
    jusitfy-content: space-between;

    width: 100%;
    max-width: 70%;
    height: 100vh;

    overflow: hidden;

    margin: 0 auto;
    padding: 15px;
  }

  .content .board{
    display: flex;
    flex-direction: column;
    width: 100%;
    max-width: 300px;
    background-color: #313131;
    padding: 15px;
    margin-left: auto;
    margin-right: auto;
    border-radius: 15px;
  }

  .content .board .card{
    padding: 15px 25px;
    background-color: #F3F3F3;
    cursor: pointer;
    margin-bottom: 15px;
    border-radius: 5px;
    text-align: center;
  }
  #first .card{
    background-color: #990000;
    color: black;
  }

  #third .card{
    background-color: #009900;
    color: white;
  }

</style>
