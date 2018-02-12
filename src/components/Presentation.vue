<template lang="pug">
  .section.hero.is-fullheight.first-section
    Header
    .hero-body
      .overlay
      .container.has-text-centered
        h3.title.is-3 Hi, my name is
        h1.title.is-name Helmer Dávila
        h3.title.is-3 Software Engineer and Fullstack Web Developer
</template>

<style lang="stylus">
@import "../stylus/media-queries"

.first-section
  background url("../assets/mac-development.jpg") center no-repeat
  background-size cover

  .overlay
    position absolute
    top 0
    left 0
    height 100%
    width 100%
    background-color #000000
    opacity 0.4

  h1, h3
    color white
  .is-name
    font-size 80px
    letter-spacing 10px
    +mobile()
      font-size 60px
</style>


<script>
import Header from './Header';

export default {
  name: 'Presentation',
  components: {
    Header,
  },
};
</script>

