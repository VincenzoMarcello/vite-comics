<script>
export default {
  methods: {
    getImageUrl(name) {
      return new URL(`../assets/${name}`, import.meta.url).href;
    },
  },
  data() {
    return {
      lineLinks: [
        {
          image: "buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },
        {
          image: "buy-comics-merchandise.png",
          text: "DC MERCHANDISE",
        },
        {
          image: "buy-comics-subscriptions.png",
          text: "SUBSCRIPTION",
        },
        {
          image: "buy-comics-shop-locator.png",
          text: "COMIC SHOP LOCATOR",
        },
        {
          image: "buy-dc-power-visa.svg",
          text: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="bg-line-blue">
    <div class="container d-flex justify-content-between align-items-center">
      <div v-for="lineLink in lineLinks">
        <div>
          <img :src="getImageUrl(lineLink.image)" alt="" class="img-line" />
        </div>
        <div>
          <p>{{ lineLink.text }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.bg-line-blue {
  min-height: 150px;
  background-color: #0282f9;
  .img-line {
    width: 60px;
    aspect-ratio: 1;
  }
}
</style>
