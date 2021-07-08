<template>
  <div class="container">
    <main class="d-flex justify-content-center flex-column text-center">
      <div class="logo my-5">
        <img src="../assets/pokedex-red.svg" alt="Pokédex" />
      </div>
      <div class="search">
        <b-form-input
          class="form-control mb-3 mt-3"
          type="text"
          placeholder="Digite o nome de um pokémon"
        />
        <b-button variant="warning" size="lg">Buscar</b-button>
      </div>
    </main>
    <div class="result">
      <div class="result-text text-center">
        <h2 class="mx-3">RESULTADO</h2>
      </div>
      <div class="card d-flex flex-row justify-content-around p-4 mb-5">
        <div class="info d-flex justify-content-around flex">
          <div class="details">
            <div class="name">
              <h2>SQUIRTLE Nº 007</h2>
              <p class="mt-3">WATER</p>
            </div>

            <div class="measures d-flex align-items-center mt-5">
              <p class="icon kg mr-5">
                <img src="../assets/balance.svg" alt="Weight" /> 9.0kg
              </p>
              <p class="icon height">
                <img src="../assets/ruler.svg" alt="Heigth" /> 0.5m
              </p>
            </div>
          </div>
          <div class="attributes">
            <p class="icon hp">
              <img src="../assets/heart.svg" alt="HP" />
              44 HP
            </p>

            <p class="icon attack">
              <img src="../assets/sword.svg" alt="Attack" />
              48 ATK
            </p>

            <p class="icon defense">
              <img src="../assets/shield.svg" alt="Defense" />
              65 DEF
            </p>

            <p class="icon speed">
              <img src="../assets/speed.svg" alt="Speed" />
              43 SPD
            </p>
          </div>
          <div class="image">
            <img src="../assets/squirtle.png" alt="Pokémon" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Livvic&family=Red+Rose:wght@400;700&display=swap");

:root {
  --bg-color: #29292e;
  --red: #ef4036;
  --yellow: #ffcb05;
  --text-color: #595959;
  --result-color: #cccccc;
  --white: #fff;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: var(--bg-color);
  font-family: "Red Rose", sans-serif;
}

.container .logo img {
  width: 100%;
  max-width: 642px;
}

main {
  width: 100%;
  max-width: 1029px;
  margin: 0 auto;
}

.search input {
  padding: 12px;
  text-align: center;
  font-size: 36px;
  color: var(--text-color);
  border-radius: 16px;
}

.search input:focus {
  border: var(--red);
  box-shadow: 0 0 0 0.2rem rgba(239, 64, 54, 0.5);
}

.search button {
  padding: 10px 75px;
  font-weight: 700;
  font-size: 36px;
  line-height: 45px;
  color: var(--text-color);
  border-radius: 16px;
}

.result-text {
  max-width: 1184px;
  width: 100%;
}

.result-text h2 {
  font-weight: bold;
  font-size: 36px;
  color: var(--result-color);
  margin: 80px 0 30px;
}

.card {
  background-color: hsl(0, 53%, 52%);
  color: var(--white);
  border-radius: 16px;
}

.card .name h2 {
  font-family: "Livvic", sans-serif;
  font-weight: bold;
  font-size: 36px;
}

.card .name p {
  background-color: hsl(0, 53%, 62%);
  width: fit-content;
  padding: 6px 22px;
  border-radius: 32px;
}

.card .info {
  flex: auto;
  align-items: center;
}

.card .info .icon {
  display: flex;
  align-items: center;
}
.card .info .icon img {
  width: 28px;
  height: 28px;
  margin-right: 8px;
}

.card .info .attributes {
  margin-top: 25px;
}

.card .image {
  background-color: #f8f8f8;
  border-radius: 16px;
}

/* .line::before {
  content: "";
  height: 1px;
  width: 454px;
  background-color: var(--result-color);
  display: block;
} */
</style>
