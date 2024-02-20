<script>
export default {
  props: {
    imgPath: String,
    title: String,
  }

}
</script>
<template>
  <h2>

  </h2>


  <div class="card">
    <img :src="imgPath" alt="">
    <h3>{{ title }}</h3>
    <p>When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper</p>
  </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/_variables.scss' as *;

.card {
  display: inline-block;
  border: none;
  padding: 0 $medium-size;
  margin: $xxlarge-size 0;


  img {
    max-width: 190px;
    height: 180px;
    object-fit: contain;
    padding-bottom: $medium-size;
  }
}
</style>
