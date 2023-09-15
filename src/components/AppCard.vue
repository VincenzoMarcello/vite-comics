<script>
export default {
  data() {
    return {
      title: "Hello world",
    };
  },

  props: {
    thumb: String,
    series: String,
  },
};
</script>

<template>
  <div class="col-3">
    <div class="card m-2" style="width: 18rem">
      <div class="card-pic">
        <img :src="thumb" class="card-img-top" alt="..." />
      </div>
      <div class="card-body">
        <p class="card-text">{{ series }}</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card-pic {
  width: 100%;
  height: 300px;
  overflow-y: hidden;

  img {
    object-fit: cover;
  }
}
</style>
