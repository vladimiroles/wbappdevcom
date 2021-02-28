<template>
  <section
    id="about"
    class="overflow-hidden"
  >
    <v-row
      class="white"
      no-gutters
    >
      <v-col
        class="pa-5"
        cols="12"
        md="6"
      >
        <base-bubble-1 style="transform: translate(5%, -5%)" />

        <base-subheading class="info--text">
          Skills
        </base-subheading>

        <v-alert
          outlined
          color="info"
        >
          <v-row
            v-for="(skill, i) in skills"
            :key="i"
            style="color: 5b5c79;"
          >
            <v-col
              class="py-1"
              cols="6"
              v-text="skill.name"
            />
          </v-row>
        </v-alert>
      </v-col>

      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/about-bg.jpg')"
          height="100%"
        />
      </v-col>
    </v-row>
  </section>
</template>

<script>
  export default {
    data: () => ({
      skills: [
        {
          name: 'JavaScript (ES6+)',
        },
        {
          name: 'HTML',
        },
        {
          name: 'CSS',
        },
        {
          name: 'SCSS',
        },
        {
          name: 'jQuery',
        },
        {
          name: 'Salesforce Commerce Cloud',
        },
        {
          name: 'VueJS',
        },
        {
          name: 'PHP',
        },
        {
          name: 'Laravel',
        },
        {
          name: 'Git',
        },
      ],
    }),
  }
</script>
