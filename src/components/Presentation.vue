<template lang="pug">
  #helmer-presentation.section.hero.is-fullheight.first-section
    Header
    .hero-body
      .overlay
      .container.has-text-centered
        h3.title.is-3 Hi, my name is
        h1.title.is-name Helmer Dávila
        h3.title.is-4 Software Engineer and Fullstack Web Developer
        .is-hidden-touch
          h2.title.is-2
            span and I build&nbsp;
            vue-typer(:text=[
              'user interfaces.',
              'landing pages.',
              'corporate websites.',
              'web applications.'])
        .is-hidden-desktop
          h3.title.is-3.text-change-mobile
            span.span-first-text and I build
            vue-typer(:text=[
              'user interfaces.',
              'landing pages.',
              'corporate websites.',
              'web applications.'])
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

  .text-change-mobile
    .span-first-text
      display block

  h1, h3, h2
    color white

  .is-name
    font-size 80px
    letter-spacing 10px
    +mobile()
      font-size 60px
</style>


<script>
import { VueTyper } from 'vue-typer';
import Header from './Header';

export default {
  name: 'Presentation',
  components: {
    Header,
    VueTyper,
  },
};
</script>

