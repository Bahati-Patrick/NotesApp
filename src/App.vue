<template>
  <main>
    <div class="overlay">
      <div class="modal">
        <textarea name="note" id="note" cols="30" rows="10"></textarea>
        <button>Add Note</button>
        <button class="close">Close</button>
      </div>
    </div>
    <div class="container">
      <header>
        <h1>Notes</h1>
        <button>+</button>
      </header>
      <div class="cards-container">
        <div class="card">
          <p class="main-text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. A illum cumque, rerum quae aliquid dolorem?</p>
          <p class="date">25/03/2024</p>
        </div>
        <div class="card">
          <p class="main-text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. A illum cumque, rerum quae aliquid dolorem?</p>
          <p class="date">25/03/2024</p>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
  main {
    height: 100vh;
    width: 100vw;
    background-color: #D0E7D2;
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
    font-weight: bold;
    margin-bottom: 25px;
    font-size: 75px;
    color: #618264;
  }

  header button {
    border: none;
    padding: 10px;
    width: 50px;
    height: 50px;
    cursor: pointer;
    background-color: #618264;
    border-radius: 100%;
    color: white;
    font-size: 20px;
  }
  
  .card {
    width: 225px;
    height: 225px;
    background-color: #79AC78;
    padding: 10px;
    border-radius: 15px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-right: 20px;
    margin-bottom: 20px;
    color: white;
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
    position:absolute;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,0.77);
    z-index: 10;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .modal {
    width: 750px;
    background-color: rgba(255, 255, 255, 0.153);
    border-radius: 10px;
    padding: 20px;
    position:relative;
    display: flex;
    flex-direction: column;
  }

  .modal button {
    padding: 10px 20px;
    font-size: 20px;
    width: 100%;
    background-color: #618264;
    border: none;
    color: white;
    cursor: pointer;
    margin-top: 15px;
    border-radius: 3px;
  }

  .modal textarea {
    border: none;
    background-color: #D0E7D2;
    border-radius: 3px;
  }

  .modal .close {
    background-color: #181818;
    margin-top: 7px;
  }
</style>