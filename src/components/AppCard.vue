<script>
export default {
  props: {
    card: Object
  }

}
</script>
<template>
  <div class="col-md-3">
    <div class="card">
      <img :src="card.imgPath" alt="">
      <h3>{{ card.title }}</h3>
      <p>{{ card.caption }}</p>
    </div>

  </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/_variables.scss' as *;

.card {
  display: inline-block;
  border: none;
  padding: 0 $medium-size;
  margin-top: $xlarge-size;
  margin-bottom: $x3large-size;


  img {
    max-width: 190px;
    height: 180px;
    object-fit: contain;
    padding-bottom: $medium-size;
  }
}
</style>
