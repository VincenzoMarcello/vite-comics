<script>
export default {
  data() {
    return {
      LineLinks: [
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

      methods: {
        getImageUrl(name) {
          return new URL(`../assets/${name}`, import.meta.url).href;
        },
      },
    };
  },
};
</script>

<template>
  <div class="bg-line-blue">
    <div class="container-links">
      <div>
        <div>
          <img :src="getImageUrl(LineLinks.image)" alt="" />
        </div>
        <div></div>
      </div>
    </div>
  </div>
</template>

<style>
.bg-line-blue {
  min-height: 150px;
  background-color: #0282f9;

  .container-links {
    max-width: 1200px;
    margin: auto;
  }
}
</style>
