<template>
  <div id="app">
    <blq-head></blq-head>
    <section-head></section-head>
    <title-head></title-head>

    <div class="page gel-wrap">
      <div class="gel-layout">

        <!-- Left -->
        <div class="gel-layout__item gel-12/12 gel-2/12@m">
          <metadata></metadata>
        </div>

        <!-- Body -->
        <div class="article gel-layout__item gel-12/12 gel-8/12@m">
          <gel-image
            src="http://placehold.it/1280x720"
            caption="Caption!"
          ></gel-image>
          <p>Lorem ipsum</p>
          <gel-image
            src="http://placehold.it/1280x720"
            caption="Caption!"
          ></gel-image>
        </div>

        <!-- Right -->
        <div class="gel-layout__item gel-12/12 gel-2/12@m">
          <more-like-this></more-like-this>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
  import BlqHead from './components/blq-head';
  import SectionHead from './components/section-head';
  import TitleHead from './components/title-head';
  import Metadata from './components/metadata';
  import GelImage from './components/gel-image';
  import MoreLikeThis from './components/more-like-this';

  export default {
    name: 'app',
    components: {
      BlqHead,
      SectionHead,
      TitleHead,
      Metadata,
      GelImage,
      MoreLikeThis,
    },
  };
</script>

<style lang="scss">
  @import './common';

  body {
    color: $purple-l1;
  }

  a {
    color: inherit;
    text-decoration: none;
  }

  .article {

    p {
      margin-top: 32px;
      margin-bottom: 0;
    }
  }

  .page {
    padding-top: 32px;
    padding-bottom: 16px;

    @include mq($from: gel-bp-m) {
      padding-bottom: 32px;
    }
  }
</style>
