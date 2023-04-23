<template>
  <q-carousel
    v-model="slide"
    transition-prev="slide-right"
    transition-next="slide-left"
    height="250px"
    arrows
    animated
    autoplay
    navigation
    infinite
    control-color="primary"
    class="rounded-borders"
  >
    <q-carousel-slide name="slide1" img-src="/images/carousel/rrlogo.jpg"/>
    <q-carousel-slide name="slide2" img-src="/images/carousel/garage-painted.jpg">
      <div class="absolute-bottom custom-caption">
        <div class="text-subtitle1">Refresh peeled paint</div>
      </div>
    </q-carousel-slide>
    <q-carousel-slide name="slide3" img-src="/images/carousel/counter-cropped.jpg">
      <div class="absolute-bottom custom-caption">
        <div class="text-subtitle1">Replace new counter top</div>
      </div>
    </q-carousel-slide>
  </q-carousel>
  <q-card class="my-card bg-secondary text-white q-mt-md q-mx-md">
      <q-card-section>
        <q-avatar>
          <img src="/images/scott.jpg">
        </q-avatar>
        <div class="text-h6">Scott Norton</div>
        <div class="text-subtitle2">Handyman</div>
      </q-card-section>

      <q-card-section>
        <p>
          With over 10 years exp. in construction, including the last 4 years as a handyman, 
          I truly enjoy what I do. I want what you want. You want the job done right, at an 
          affordable price, completed in a timely fashion. No matter what size your project is, 
          I will treat your home as if it is my own.
        </p>
        <p>
          Call/text anytime for a free quote and appointment time.
        </p>
      </q-card-section>

      <q-separator dark />

      <q-card-actions>
        <q-btn flat href="tel://214-957-7388">Call Me</q-btn>
        <q-btn flat href="sms:+12149577388">Text Me</q-btn>
      </q-card-actions>
    </q-card>
</template>

<style lang="sass" scoped>
.custom-caption
  text-align: center
  padding: 12px
  margin-bottom: 50px
  color: white
  background-color: rgba(0, 0, 0, .4)
</style>

<script>
import { ref } from 'vue'
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  setup () {
    return {
      slide: ref('slide1'),
      lorem: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos praesentium libero ab nemo provident incidunt ducimus iusto perferendis porro earum. Totam, numquam?'
    }
  }
})

</script>
