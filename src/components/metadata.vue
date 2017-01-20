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
      margin-top: 0;
      margin-bottom: 0;
      overflow: hidden; // Clearfix

      li {
        float: left;
        margin-left: 16px;

        &:first-child {
          margin-left: 0;
          margin-right: 16px;
        }

        @include mq($from: gel-bp-m) {
          float: none;
          margin-left: 0;

          &:first-child {
            margin-right: 0;
          }
        }
      }

      a {
        text-decoration: underline;
      }
    }
  }
</style>
