<template lang="pug">
  .section
    .container
      h1.title.is-1.has-text-centered My stack
      .level
        .level-item
          .icon-container
            i.fab.fa-js-square.fa-fw.fa-3x
          h4.title.is-4 Javascript
          span Backend / Frontend
        .level-item
          .icon-container
            i.fab.fa-php.fa-fw.fa-3x
          h4.title.is-4 PHP
          span Backend
        .level-item
          .icon-container
            i.fab.fa-css3-alt.fa-fw.fa-3x
          h4.title.is-4 HTML + CSS
          span Frontend
        .level-item
          .icon-container
            i.fab.fa-linux.fa-fw.fa-3x
          h4.title.is-4 Linux
          span Server deployment
</template>

<style lang="stylus" scoped>
@import '../stylus/variables'

.section
  h1.title
    margin-bottom 1em

.level-item
  flex-direction column
  .icon-container
    color primary-color
    margin-bottom 1.3em
</style>
