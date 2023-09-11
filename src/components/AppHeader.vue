<script>
export default {
  data() {
    return {
      links: [
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ],
    };
  },
};
</script>

<template>
  <header>
    <div class="container">
      <div class="row">
        <div class="img-container">
          <img src="/dc-logo.png" alt="" />
        </div>
        <ul>
          <li v-for="link in links">{{ link }}</li>
        </ul>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
header {
  background-color: #ffffff;

  .container {
    max-width: 1200px;
    margin: auto;

    .row {
      display: flex;
      justify-content: space-between;
      align-items: center;

      .img-container {
        padding: 0.5rem 0;
      }

      ul {
        display: flex;
        gap: 1rem;
        list-style: none;

        li {
          font-weight: bolder;
          cursor: pointer;

          &:hover {
            color: #0282f9;
          }
        }
      }
    }
  }
}
</style>
