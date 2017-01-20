<template>
  <div class="more-like-this">
    <h3>More like this</h3>
    <ul>
      <li><a href="#">Starguide: January 2017</a></li>
      <li><a href="#">Pete Lawrence's Moon guides</a></li>
      <li><a href="#">How do telescopes work?</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {

    };
  },
};
</script>

<style lang="scss">
  @import '../common';

  .more-like-this {
    border-top: 1px solid;
    margin-top: 32px;

    @include mq($from: gel-bp-m) {
      margin-top: 0;
    }

    ul {
      @extend %list;
    }

    h3 {
      @include gel-typography('double-pica-bold');
      padding-top: 16px;
      margin-top: 0;
      margin-bottom: 16px;
    }

    a {
      @include gel-typography('pica-bold');
      font-weight: bold;
    }
  }
</style>
