<template>
  <section
    id="welcome"
    class="overflow-hidden mt-8 mt-md-0"
  >
    <v-row no-gutters>
      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/welcome-bg.jpg')"
          height="100vh"
        />
      </v-col>

      <v-col
        class="align-content-space-between layout wrap"
        cols="12"
        md="6"
      >
        <base-bubble-1
          style="transform: rotate(180deg) translateY(25%)"
        />

        <v-row
          align="center"
          justify="center"
        >
          <v-col
            cols="12"
            md="6"
            class="pl-8 pl-md-0"
          >
            <base-heading>Hello!</base-heading>
            <base-text>
            My name is Vladimir. I am self-motivated front-end developer with 4 years of commercial experience working on multiple projects. <br>
            You can learn more about me by downloading my CV below.
            </base-text>
            <v-btn
              color="secondary"
              rounded
              :href="downloadLink"
              download
            >
            Download CV
            </v-btn>
          </v-col>
        </v-row>

        <base-bubble-2
          style="transform: rotate(180deg) translate(-200px, -15%)"
        />
      </v-col>
    </v-row>
  </section>
</template>

<script>
  export default {
    data: () => ({
      downloadLink: 'files/cv-vladimir-olesko-fd-developer.pdf',
    }),
  }
</script>
