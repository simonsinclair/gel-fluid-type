<template>
  <div class="title-head">
    <div class="gel-wrap">
      <div class="gel-layout">
        <div class="gel-layout__item gel-2/12">
          <contributor
            src="http://placehold.it/64x64"
            name="Dr Maggie Aderin-Pocock"
            role="Presenter"
          ></contributor>
        </div>
        <div class="gel-layout__item gel-8/12">
          <h2>Beam me up: These pillars of light are like something out of Star Trek</h2>
          <p>A description goes here and would be about this long, but could be longer depending on how descriptive it is and how much was written.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import Contributor from './contributor';

  export default {
    components: {
      Contributor,
    },
    data() {
      return {

      };
    },
  };
</script>

<style lang="scss">
  @import '../common';

  .title-head {
    background-color: $purple-l2;
    color: #FFF;
    padding-top: 32px;
    padding-bottom: 32px;

    h2 {
      @include gel-typography('trafalgar-bold');
    }
    p {
      @include gel-typography('great-primer');
    }
  }
</style>
