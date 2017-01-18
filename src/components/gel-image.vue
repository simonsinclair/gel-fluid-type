<template>
  <figure class="gel-image">
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

  .gel-image {
    margin: 0;

    img {
      max-width: 100%;
      vertical-align: middle;
    }

    figcaption {
      @include gel-typography('brevier');
      color: $purple-l3;
      padding-top: 16px;
    }
  }
</style>
