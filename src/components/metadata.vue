<template>
  <div class="metadata">
    <ul>
      <li>09 January 2017</li>
      <li><a href="#">Aurora</a></li>
      <li><a href="#">Canada</a></li>
      <li><a href="#">Natural phenomena</a></li>
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

  .metadata {

    ul {
      @extend %list;

      a {
        text-decoration: underline;
      }
    }
  }
</style>
