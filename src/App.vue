<template lang="pug">
  #app
    Presentation
    MyStack
    WhatDo
    Footer
</template>

<style lang="sass">
@import "~bulma/sass/utilities/initial-variables";
$primary: black;
$family-primary: 'Quicksand', sans-serif;
@import "~bulma";
</style>

<style lang="stylus">
.button
  border-radius 100px
  padding 0.7em 1.5em
  box-shadow 0 10px 20px rgba(0, 0, 0, 0.2)
  font-weight 700
  line-height 1
  height auto
</style>


<script>
import Presentation from './components/Presentation';
import Footer from './components/Footer';
import WhatDo from './components/WhatDo';
import MyStack from './components/MyStack';

export default {
  name: 'App',
  components: {
    Presentation,
    MyStack,
    WhatDo,
    Footer,
  },
};
</script>
