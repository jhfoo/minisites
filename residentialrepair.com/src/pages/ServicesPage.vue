<template>
  <q-card class="my-card bg-secondary text-white q-mt-md q-mx-md">
      <q-card-section>
        <div class="text-h6">Services and Specialties</div>
      </q-card-section>

      <q-card-section>
        <p>
          I have 10 years experience as a builder, drywall technician, 
          painter, carpenter, as well as some plumbing and electrical. 
          I enjoy working hard for my customers making sure they are more 
          than satisfied with the service I provided. Being self employed 
          I can afford to offer a lesser price than most without compromising 
          quality . I collect payment when you are happy with my results.
        </p>
        <p>
          Services I offer include:
          <ul>
            <li>Painting interior/exterior</li>
            <li>Repair drywall and texture</li>
            <li>Carpentry- repair siding</li>
            <li>Build patio covers/pergolas</li>
            <li>Install shelves</li>
            <li>Mount TVs</li>
            <li>Install/repair appliances</li>
            <li>Replace faucets</li>
            <li>Fix plumbing leaks</li>
            <li>Fix doors</li>
            <li>Replace mailboxes</li>
            <li>Electrical-install lights and ceiling fans</li>
            <li>Fix doors</li>
            <li>Move outlets</li>
            <li>Designed many flower beds , trim and prune trees , mulch , even pull weeds</li>
          </ul>  
          and many more. 
        </p>
        <p>
          I look forward to the opportunity of working with you on your project 
          no matter what size.
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
