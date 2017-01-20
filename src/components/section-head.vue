<template>
  <div class="section-head">
    <div class="gel-wrap">
      <div class="gel-layout gel-layout--center">
        <div class="gel-layout__item gel-12/12 gel-6/12@m">
          <h1>The Sky at Night</h1>
        </div>
      </div>
    </div>
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

  .section-head {
    background-color: $purple-l1;
    padding-top: 16px;
    padding-bottom: 16px;
    -webkit-font-smoothing: antialiased;

    h1 {
      // @include gel-typography('canon');
      font-size: 5vw;
      line-height: 1;

      color: #FFF;
      margin-top: 0;
      margin-bottom: 0;
    }
  }
</style>
