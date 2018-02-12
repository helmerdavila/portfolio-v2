<template lang="pug">
  .footer
    .container
      .content.has-text-centered
        a.rounded-link
          i.fab.fa-linkedin-in.fa-fw
        p
          span &copy
          span {{ ` ${actualDate}` }}
</template>

<style lang="stylus">
.footer
  background black
  color: white
  .rounded-link
    padding 0.5em
    background white
    color black
    border-radius 50%
    margin 0 0.5em
  p
    margin-top 20px
</style>


<script>
export default {
  data() {
    return {
      actualDate: null,
    };
  },
  mounted() {
    const actualDate = new Date();
    this.actualDate = actualDate.getFullYear();
  },
};
</script>

