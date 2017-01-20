<template>
  <div class="contributor">
    <slot></slot>
    <div class="contributor__text">
      <p class="contributor__name">{{name}}</p>
      <p class="contributor__role">{{role}}</p>
    </div>
  </div>
</template>

<script>
  export default {
    props: ['path', 'name', 'role'],
    data() {
      return {

      };
    },
  };
</script>

<style lang="scss">
  @import '../common';

  .contributor img,
  .contributor__text {
    float: left;

    @include mq($from: gel-bp-m) {
      float: none;
    }
  }
  .contributor {
    overflow: hidden; // Clearfix

    img {
      border-radius: 50%;
      height: 48px;
      margin-right: 8px;
      width: 48px;
    }
  }

  .contributor__text {}

  .contributor__name,
  .contributor__role {
    @include gel-typography('pica-bold');
    margin-top: 2px;
    margin-bottom: 2px;
  }

  .contributor__role {
    font-weight: normal;
  }
</style>
