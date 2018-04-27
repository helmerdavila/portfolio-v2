<template lang="pug">
  section#helmer-projects.section.section-projects
    .container
      h1.title.is-1.has-text-centered My projects
      carousel(:autoplay="true" paginationColor="#686469" :perPage="3")
        template(v-for="slide in slides")
          slide
            .card
              .card-image
                figure.image
                  img(:src="slide.image")
                  .overlay
              .card-content.has-text-centered
                h3.is-3.title {{ slide.name }}
                .field.is-grouped
                  .control
                    .tags.has-addons
                      span.tag Backend
                      span.tag.is-black {{ slide.backend }}
                  .control
                    .tag.has-addons
                      span.tag Frontend
                      span.tag.is-black {{ slide.frontend }}
              .card-footer
                .card-footer-item
                  a.button.is-small.is-rounded.is-primary(:href="slide.url" target="_blank")
                    | Visit site
</template>

<style lang="stylus" scoped>

</style>


<script>
import { Carousel, Slide } from 'vue-carousel';
import AmbreaImage from '../assets/ambrea_mockup.png';
import BipolarImage from '../assets/bipolar_mockup.png';
import FitnessPass from '../assets/fitnesspass_mockup.png';
import SpoonTop from '../assets/spoontop_mockup.png';

export default {
  name: 'Projects',
  components: {
    Carousel,
    Slide,
  },
  data() {
    return {
      slides: [
        {
          name: 'Ambrea',
          image: AmbreaImage,
          url: 'http://ambrea.pe',
          backend: 'Laravel',
          frontend: 'Vue, Vuex',
        },
        {
          name: 'Bipolar',
          image: BipolarImage,
          url: 'http://bipolar.com.pe',
          backend: 'Laravel',
          frontend: 'React',
        },
        {
          name: 'Fitnesspass',
          image: FitnessPass,
          url: 'http://fitnesspass.pe',
          backend: 'Express',
          frontend: 'React',
        },
        {
          name: 'Spoontop',
          image: SpoonTop,
          url: 'http://spoontop.com',
          backend: 'Laravel',
          frontend: 'Angular, Ionic',
        },
      ],
    };
  },
};
</script>
