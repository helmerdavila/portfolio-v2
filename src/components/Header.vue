<template lang="pug">
  nav.navbar.is-fixed-top(:class="{ 'is-scrolled': scrolled }")
    .navbar-brand
      a.navbar-item(href="https://bulma.io")
        i.fas.fa-h-square.fa-2x
      .navbar-burger.burger(data-target="navbarExampleTransparentExample")
        span
        span
        span
    #navbarExampleTransparentExample.navbar-menu
      .navbar-start
        a.navbar-item(href="#") Who am I
        a.navbar-item(href="#") My stack
        a.navbar-item(href="#") What I do
        a.navbar-item(href="#") Experience
      .navbar-end
        .navbar-item
          .field.is-grouped
            p.control
              a.button.is-primary(href="https://github.com/jgthms/bulma/archive/0.5.1.zip", :class="{ 'is-inverted': !scrolled, 'is-outlined': !scrolled }")
                span.icon
                  i.fas.fa-download
                span Download CV
</template>

<style lang="stylus" scoped>
a.navbar-item
  color white
  &:hover
    background-color transparent
    color white

.is-scrolled
  background white
  a.navbar-item
    color black
</style>


<script>
export default {
  name: 'Header',
  data() {
    return {
      scrolled: false,
    };
  },
  methods: {
    handleScroll() {
      this.scrolled = window.scrollY > 0;
    },
  },
  created() {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed() {
    window.removeEventListener('scroll', this.handleScroll);
  },
};
</script>
