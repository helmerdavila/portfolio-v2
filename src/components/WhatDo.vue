<template lang="pug">
.section.what-i-do
  .container
    h1.title.is-1.has-text-centered What I do
    .columns
      .column
        .service.has-text-centered
          span.the-icon
            i.fab.fa-chrome.fa-3x.fa-fw
          .content
            h3 Frontend Development
            p Code useful and dynamic interfaces with cross-browser compatibility.
      .column
        .service.has-text-centered
          span.the-icon
            i.fas.fa-code.fa-3x.fa-fw
          .content
            h3 Backend Development
            p Code the requirements and restrictions for the business.
      .column
        .service.has-text-centered
          span.the-icon
            i.fas.fa-server.fa-3x.fa-fw
          .content
            h3 Server deployment
            p Upload new changes in my apps with tools for automated deployments.
</template>

<style lang="stylus">
@import '../stylus/variables'

.what-i-do
  background-color #F0F0F0

  h1.title
    margin-bottom 1.5em

  .service
    width 100%
    background white
    border-radius 4px
    padding 48px 20px
    box-shadow 0px 0px 10px rgba(0, 0, 0, 0.2)
    transition all 0.3s ease-in-out 0s

    &:hover
      box-shadow 0px 0px 30px rgba(0, 0, 0, 0.2)

    span.the-icon
      display block
      color primary-color

    h3
      margin-top 1.5em
      text-transform uppercase
</style>

