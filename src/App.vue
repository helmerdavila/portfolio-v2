<template lang="pug">
  #app
    Presentation
    AboutMe
    WhatDo
    MyStack
    Projects
    Footer
</template>

<style lang="scss">
@import '~bulma/sass/utilities/initial-variables';
$primary: black;
$family-primary: 'Quicksand', sans-serif;
@import '~bulma';
</style>

<style lang="stylus">
@import './stylus/helmer-portfolio'
</style>


<script>
import AboutMe from './components/AboutMe';
import Presentation from './components/Presentation';
import Footer from './components/Footer';
import WhatDo from './components/WhatDo';
import MyStack from './components/MyStack';
import Projects from './components/Projects';

export default {
  name: 'App',
  components: {
    Presentation,
    AboutMe,
    MyStack,
    WhatDo,
    Projects,
    Footer,
  },
};
</script>
