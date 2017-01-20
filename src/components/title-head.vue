<template>
  <div class="title-head">
    <div class="gel-wrap">
      <div class="gel-layout">
        <div class="gel-layout__item gel-12/12 gel-2/12@m">
          <contributor
            name="Dr Maggie Aderin-Pocock"
            role="Presenter"
          >
            <img src="~assets/maggie.jpg" class="contributor__avatar" />
          </contributor>
        </div>
        <div class="gel-layout__item gel-12/12 gel-8/12@m">
          <h2>Beam me up: These pillars of light are like something out of Star Trek</h2>
          <p>Canadian man captures stunning photographs of incredibly rare natural phenomenon in the freezing night sky.</p>
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
    -webkit-font-smoothing: antialiased;

    h2 {
      @include gel-typography('trafalgar-bold');

      @include mq($from: gel-bp-m) {
        margin-top: 0;
      }
    }
    p {
      @include gel-typography('great-primer');
      margin-bottom: 0;
    }
  }
</style>
