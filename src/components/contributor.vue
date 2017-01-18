<template>
  <div class="contributor">
    <img :src="src" alt="" class="contributor__avatar" />
    <p class="contributor__name">{{name}}</p>
    <p class="contributor__role">{{role}}</p>
  </div>
</template>

<script>
export default {
  props: ['src', 'name', 'role'],
  data() {
    return {

    };
  },
};
</script>

<style lang="scss">
  @import '../common';

  .contributor {

    img {
      border-radius: 50%;
    }
  }

  .contributor__name,
  .contributor__role {
    @include gel-typography('pica-bold');
  }

  .contributor__role {
    font-weight: normal;
  }
</style>
