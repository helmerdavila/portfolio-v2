<template lang="pug">
  .footer
    .container
      .content.has-text-centered
        a.rounded-link(href="https://www.linkedin.com/in/helmerdavila/" target="_blank")
          i.fab.fa-linkedin-in.fa-fw
        a.rounded-link(href="https://www.github.com/helmerdavila/" target="_blank")
          i.fab.fa-github.fa-fw
        p
          span &copy Handmade by me
          span {{ ` ${actualDate}` }}
</template>

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
