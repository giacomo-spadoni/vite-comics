<script>
export default {
  props: ['fumetto'],
  methods: {
    getImage(nomefile) {
      return new URL(`${nomefile}`, import.meta.url);
    },
  },
};
</script>
<template>
  <div class="card">
    <div class="img-container">
      <img :src="getImage(fumetto.thumb)" alt="" />
    </div>
    <div class="title">{{ fumetto.series }}</div>
  </div>
</template>
<style scoped>
.card {
  width: 15%;
  margin-bottom: 2rem;
}

.img-container img {
  width: 100%;
  aspect-ratio: 1;
  object-fit: cover;
}

.title {
  font-size: 16px;
}
</style>
