<template lang="pug">
  section#helmer-whatido.section.what-i-do
    .container
      h1.title.is-1.has-text-centered What I do
      .columns
        .column
          .service.has-text-centered
            span.the-icon
              i.fab.fa-chrome.fa-3x.fa-fw
            .content
              h3 Frontend Development
              p
              | I design in the browser with HTML(5), CSS(3) and a touch of JavaScript.
              | I love coding things from scratch, but I can work with front-end CSS
              | frameworks like Bootstrap or Bulma too.
        .column
          .service.has-text-centered
            span.the-icon
              i.fas.fa-code.fa-3x.fa-fw
            .content
              h3 Backend Development
              p
                | Code the requirements and restrictions for the business, using backend frameworks
                | with good scalability option and quick development of new features.
        .column
          .service.has-text-centered
            span.the-icon
              i.fas.fa-server.fa-3x.fa-fw
            .content
              h3 Server management
              p
                | Upload new changes in apps with tools for automated deployments. Setting
                | testing and production environments, avoiding security mistakes.
</template>

<style lang="stylus">
@import '../stylus/variables';

.what-i-do {
  background-color: #F0F0F0;

  h1.title {
    margin-bottom: 1.5em;
  }

  .service {
    width: 100%;
    background: white;
    border-radius: 4px;
    padding: 48px 20px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
    transition: all 0.3s ease-in-out 0s;

    &:hover {
      box-shadow: 0px 0px 30px rgba(0, 0, 0, 0.2);
    }

    span.the-icon {
      display: block;
      color: primary-color;
    }

    h3 {
      margin-top: 1.5em;
      text-transform: uppercase;
    }
  }
}
</style>
