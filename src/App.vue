<template>
  <div id="app">
    <blq-head></blq-head>
    <section-head></section-head>
    <title-head></title-head>

    <div class="page gel-wrap">
      <div class="gel-layout">

        <!-- Left -->
        <div class="gel-layout__item gel-12/12 gel-3/12@m">
          <metadata></metadata>
        </div>

        <!-- Body -->
        <div class="article gel-layout__item gel-12/12 gel-9/12@m">
          <gel-image caption="Caption!">
            <img src="~assets/pillar-lights.jpg" alt="">
          </gel-image>

          <p>A photographer in Canada man was surprised to wake up in the middle of the night to see beams of brightly coloured lights shooting up into the sky.</p>

          <p>"We can blame the two-year-old. He started crying at 1:30 a.m., so I got up and soothed him ... and out the window I had the perfect view of these dancing lights in the sky," said Timothy Joseph Elzinga.</p>

          <p>"I had to investigate. I got some pants on and ran outside and took some photos."</p>

          <p>Phasellus vitae lacus mi. Vestibulum at rhoncus libero, ut pellentesque lacus. Cras ut mollis risus. Proin mollis nunc sed lectus ullamcorper, in viverra ante elementum. Cras vitae turpis volutpat, consectetur erat vitae, luctus purus. Vivamus non rutrum odio. Nam lorem nibh, auctor nec rhoncus tempus, facilisis vitae libero. In et efficitur metus, at lacinia dolor. Maecenas et vestibulum tortor. Nullam mollis nulla vel aliquam condimentum.</p>

          <p>Vestibulum pharetra eget odio a rhoncus. Integer diam tellus, imperdiet et ultrices id, laoreet sit amet ligula. Cras nec erat magna. Phasellus eros tellus, aliquet vitae nisl ac, sodales consectetur tortor. Cras eget massa scelerisque ipsum cursus mattis id vitae velit. Integer molestie magna sit amet libero vestibulum, ut bibendum sem convallis. Nulla sit amet felis euismod, finibus ipsum sed, aliquet ante. Morbi lorem tellus, semper vitae elit aliquet, fermentum bibendum magna. Vivamus pellentesque egestas metus eu vehicula. Nunc eleifend faucibus nibh ut sollicitudin. Integer diam orci, pharetra ac fermentum ut, convallis eu ipsum. Suspendisse potenti. Proin congue leo eu eros convallis imperdiet. Fusce tristique fermentum egestas. Suspendisse ipsum massa, efficitur sed mi at, auctor imperdiet ipsum.</p>

          <p>Duis ac ornare arcu. Donec posuere lacus et neque facilisis semper. Sed commodo sed nulla vitae mollis. Maecenas ac pellentesque lacus. Ut mattis convallis mattis. Nam facilisis, tortor sed aliquet placerat, nulla leo laoreet nisi, at rhoncus orci quam ut lectus. Vivamus dapibus ex mauris, eu sollicitudin ante euismod nec. Mauris elementum libero magna. Suspendisse vehicula placerat eleifend.</p>

          <gel-image caption="Caption!">
            <img src="~assets/aurora.jpg" alt="">
          </gel-image>

          <p>Aliquam pellentesque aliquet lorem, sed elementum diam sodales et. Sed ut leo condimentum, venenatis massa vitae, feugiat massa. Nunc in orci ac ex finibus efficitur et at libero. Proin non faucibus sapien. Duis eu sodales metus, at sollicitudin mauris. Praesent pellentesque, justo ac laoreet dictum, risus mi condimentum turpis, eget luctus ante ipsum non neque. Duis a quam aliquet, tincidunt nibh at, mollis nisi. Vivamus faucibus interdum nisl vel dignissim.</p>

          <p>Donec sollicitudin, dui a tincidunt ornare, nibh enim ullamcorper quam, nec consequat risus diam quis mi. Morbi tortor velit, ultrices et maximus vitae, egestas nec erat. Integer quis nibh vel nunc venenatis pulvinar. Interdum et malesuada fames ac ante ipsum primis in faucibus. Fusce egestas varius sapien, sit amet vehicula ante vehicula a. Sed interdum, velit nec tristique fermentum, dui mauris mollis ligula, et consectetur urna magna a lectus. Nulla eu semper mauris, et feugiat nisl. Sed eget volutpat erat. Vestibulum et ex sit amet odio laoreet vestibulum at quis nunc.</p>

        </div>

        <!-- Right -->
        <div class="gel-layout__item gel-12/12">
          <div class="mlt">
            <more-like-this></more-like-this>
          </div>
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
    font-size: 3vw;
    line-height: 1.5;
  }

  a {
    color: inherit;
    text-decoration: none;

    &:hover {
      color: #008550;
    }
  }

  .article {

    p {
      margin-top: 16px;
      margin-bottom: 0;
    }

    p ~ .gel-image {
      margin-top: 16px;
    }
  }

  .page {
    padding-top: 32px;
    padding-bottom: 16px;

    @include mq($from: gel-bp-m) {
      padding-bottom: 32px;
    }
  }

  .mlt {
    padding-left: 0;

    @include mq($from: gel-bp-m) {
      padding-left: 25%;
    }
  }
</style>
