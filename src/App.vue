<script setup>

</script>

<template>
  <main>
    <div class="overlay">
      <div class="modal">
        <textarea name="notes" id="notes" cols="30" rows="10"></textarea>
        <button>Add Note</button>
      </div>
    </div>

    <div class="container">
      <header>
        <h1>Notes</h1>
        <button>+</button>
      </header>
      <div class="cards-container">
        <div class="card">
          <p class="main-text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Natus ab, adipisci quae maxime iste incidunt?</p>
          <p class="date">22/02/2024</p>
        </div>
        <div class="card">
          <p class="main-text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Natus ab, adipisci quae maxime iste incidunt?</p>
          <p class="date">22/02/2024</p>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
  main {
    background-color: rgb(255, 255, 255);
    height: 100vh;
    width: 100vw;
  }

  .container {
    max-width: 1000px;
    padding: 10px;
    margin: 0 auto;
  }

  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  h1 {
    color: rgb(0, 0, 0);
    font-weight: bold;
    margin-bottom: 25px;
    font-size: 75px;
  }

  header button {
    border: none;
    padding: 10px;
    width: 50px;
    height: 50px;
    cursor: pointer;
    background-color: bisque;
    border-radius: 100%;
    color: rgb(0, 0, 0);
    font-size: 20px;
  }

  .card {
    width: 225px;
    height:225px;
    background-color: bisque;
    padding: 10px;
    border-radius: 15px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-right: 20px;
    margin-bottom: 20px;
  }

  .date {
    font-size: 12.5px;
    font-weight: bold;
  }

  .cards-container {
    display: flex;
    flex-wrap: wrap;
    
  }

  .overlay {
    position: absolute;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.77);
    z-index: 10;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .modal {
    width: 750px;
    background-color: white;
    border-radius: 10px;
    padding: 30px;
    position: relative;
    display: flex;
    flex-direction: column;
  }

</style>
