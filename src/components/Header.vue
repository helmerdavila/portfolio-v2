<template lang="pug">
  nav.navbar.is-fixed-top(:class="{ 'is-scrolled': scrolled }")
    .navbar-brand
      a.navbar-item(href="/")
        i.fas.fa-h-square.fa-2x
      .navbar-burger.burger(@click="menuIsActive = !menuIsActive")
        span
        span
        span
    .navbar-menu(:class="{ 'is-active': menuIsActive }")
      .navbar-start
        a.navbar-item(href="#" v-scroll-to="'#helmer-presentation'") Who am I
        a.navbar-item(href="#" v-scroll-to="'#helmer-aboutme'") About me
        a.navbar-item(href="#" v-scroll-to="'#helmer-whatido'") What I do
        a.navbar-item(href="#" v-scroll-to="'#helmer-mystack'") My stack
        a.navbar-item(href="#" v-scroll-to="'#helmer-projects'") My projects
      .navbar-end
        .navbar-item
          .field.is-grouped
            p.control
              a.button.is-primary(href="https://www.dropbox.com/s/xubgx2iei31njza/Helmer_CV.pdf?dl=0", :class="{ 'is-inverted is-outlined': !scrolled && !menuIsActive }")
                span.icon
                  i.fas.fa-download
                span Download CV
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      scrolled: false,
      menuIsActive: false,
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
