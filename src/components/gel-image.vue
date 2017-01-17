<template>
  <figure>
    <img :src="src" alt="" />
    <figcaption>{{caption}}</figcaption>
  </figure>
</template>

<script>
export default {
  props: ['src', 'caption'],
  data() {
    return {

    };
  },
};
</script>

<style lang="scss">
  @import '../common';

  img {
    max-width: 100%;
  }
</style>
