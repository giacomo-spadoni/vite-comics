<script></script>

<template>
  <header>
    <section>
      <div class="container">
        <div class="logo">
          <img src="../assets/dc-logo.png" alt="" />
        </div>
        <ul>
          <li>CHARACTERS</li>
          <li>COMICS</li>
          <li>MOVIES</li>
          <li>TV</li>
          <li>GAMES</li>
          <li>COLLECTIBLES</li>
          <li>VIDEOS</li>
          <li>FANS</li>
          <li>NEWS</li>
          <li>SHOP</li>
        </ul>
      </div>
    </section>
  </header>
</template>

<style scoped>
header {
  background-color: rgb(235, 235, 235);
  width: 100%;
  position: fixed;
  z-index: 1;
}

.container {
  max-width: 1400px;
  margin: 0 auto;
  color: black;
  font-weight: 600;
  min-height: 6rem;
  display: flex;
  width: 100%;
  align-items: center;
}

img {
  width: 60px;
}

.logo {
  width: 30%;
}

ul {
  width: 70%;
  display: flex;
  justify-content: space-between;
}
</style>
