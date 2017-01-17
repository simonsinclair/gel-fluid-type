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

</style>
