<template>
  <div>
    <v-btn
      v-for="(item, i) in items.slice(0, large ? items.length : 3)"
      :key="i"
      fab
      class="ma-2"
      :href="item.href"
      color="info"
      :small="!large"
    >
      <v-icon
        dark
        v-text="item.icon"
      />
    </v-btn>
  </div>
</template>

<script>
  export default {
    props: {
      large: {
        type: Boolean,
        default: false,
      },
    },

    data: () => ({
      items: [
        {
          name: 'Skype',
          icon: 'mdi-skype',
          href: 'skype:vladimiroles?chat',
        },
        {
          name: 'Email',
          icon: 'mdi-email',
          href: 'mailto:vladimiroles@gmail.com',
        },
      ],
    }),
  }
</script>
