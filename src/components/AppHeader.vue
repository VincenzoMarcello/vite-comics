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
  <div class="container">
    <div class="d-flex justify-content-between align-items-center">
      <div class="img-container">
        <img src="/dc-logo.png" alt="" />
      </div>
      <ul>
        <li v-for="link in links">{{ link }}</li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.img-container {
  padding: 0.5rem 0;
}

ul {
  display: flex;
  gap: 1rem;
  margin-bottom: 0;
  list-style: none;

  li {
    font-weight: bolder;
    cursor: pointer;

    &:hover {
      color: #0282f9;
    }
  }
}
</style>
