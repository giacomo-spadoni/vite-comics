<script>
export default {
  data() {
    return {
      listBuy: [
        {
          img: 'buy-comics-digital-comics.png',
          description: 'DIGITAL COMICS',
        },
        {
          img: 'buy-comics-merchandise.png',
          description: 'DC MERCHANDISE',
        },
        {
          img: 'buy-comics-subscriptions.png',
          description: 'SUBSCRIPTION',
        },
        {
          img: 'buy-comics-shop-locator.png',
          description: 'COMIC SHOP LOCATOR',
        },
        {
          img: 'buy-dc-power-visa.svg',
          description: 'DC POWER VISA',
        },
      ],
    };
  },
  methods: {
    getImage(nomefile) {
      return new URL(`../assets/${nomefile}`, import.meta.url);
    },
  },
};
</script>
<template>
  <footer>
    <section class="list">
      <div class="container-list">
        <div v-for="(buy, i) in listBuy" class="buy-comics">
          <img :src="getImage(buy.img)" alt="" />
          <div>{{ buy.description }}</div>
        </div>
      </div>
    </section>
    <section class="list-background">
      <div class="container-list-background">
        <div class="col-4">
          <ul>
            <li class="title">DC COMICS</li>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
            <li class="title">DC COMICS</li>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
          <ul>
            <li class="title">DC</li>
            <li>Terms Of Use</li>
            <li>Privacy Policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscription</li>
            <li>Talent Workshop</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
          <ul>
            <li class="title">Sites</li>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>
        </div>
        <div class="img-container">
          <img src="../assets/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </section>
    <section class="contacts">
      <div class="container-contacts">
        <button>SIGN-UP NOW!</button>
        <div class="follow">
          <div>FOLLOW US</div>
          <img src="../assets/footer-facebook.png" alt="" />
          <img src="../assets/footer-twitter.png" alt="" />
          <img src="../assets/footer-youtube.png" alt="" />
          <img src="../assets/footer-pinterest.png" alt="" />
          <img src="../assets/footer-periscope.png" alt="" />
        </div>
      </div>
    </section>
  </footer>
</template>
<style scoped>
footer {
  width: 100%;
}

.list {
  background-color: #0282f9;
  width: 100%;
  font-weight: 600;
}

.container-list {
  max-width: 1400px;
  margin: 0 auto;
  min-height: 10rem;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.buy-comics {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.buy-comics img {
  height: 4rem;
  max-width: 4rem;
}

.list-background {
  background-image: url(../assets/footer-bg.jpg);
  width: 100%;
  height: 25rem;
  overflow: hidden;
}

.container-list-background {
  max-width: 1400px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}

.col-4 {
  width: calc(100% / 12 * 4);
  display: flex;
  margin-top: 2rem;
  margin-bottom: 4rem;
}

.img-container {
  width: 45%;
  position: relative;
}

.img-container > img {
  position: absolute;
  top: -5rem;
}

ul {
  margin-right: 1rem;
}

li {
  color: rgb(150, 150, 150);
}

.title {
  padding: 1rem 0;
  font-weight: bold;
  color: white;
}

.container-contacts {
  max-width: 1400px;
  margin: 0 auto;
  display: flex;
  min-height: 4.5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

button {
  padding: 0.8rem;
  background-color: #242424;
  border: 2px solid #0282f9;
}

.follow {
  color: #0282f9;
  font-weight: bold;
  display: flex;
  gap: 1rem;
  align-items: center;
}
</style>
