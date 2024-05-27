<script>
import SeriesList from './SeriesList.vue';
export default {
  components: {
    SeriesList,
  },
};
</script>
<template>
  <main>
    <section>
      <div class="background">
        <div class="title">CURRENT SERIES</div>
      </div>
      <SeriesList />
      <div class="button-load">
        <div class="title">LOAD MORE</div>
      </div>
    </section>
  </main>
</template>
<style scoped>
main {
  padding-top: 6rem;
}

.background {
  /* padding-top: 6rem; */
  width: 100%;
  height: 25rem;
  background-image: url(../assets/jumbotron.jpg);
  position: relative;
}

.background .title {
  font-size: 25px;
  font-weight: bold;
  background-color: #0282f9;
  padding: 0.4rem 1.3rem;
  position: absolute;
  bottom: -1.5rem;
  left: 15rem;
}

.button-load {
  display: flex;
  justify-content: center;
  margin-bottom: 2rem;
}

.title {
  font-weight: bold;
  background-color: #0282f9;
  padding: 0.4rem 4rem;
  display: inline-block;
  text-align: center;
}
</style>
